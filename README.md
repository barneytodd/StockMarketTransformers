# 📊 Machine Learning and Transformer Networks in Stock Market Prediction
## Barney Todd
### March 2024

###  Project Overview  
A research-focused project exploring whether transformer networks can be used to predict or assist in predicting stock returns. <br>
The project integrates in-depth neural network analysis, sequence modeling, and attention-based architectures to study robustness and correlation in financial time series, by studying:

- **Neural Network Foundations:** Comprehensive exploration of fully connected networks, training, optimization, and evaluation.  
- **Sequence Models:** Investigated RNNs and LSTMs, comparing their capabilities to Transformers in modeling temporal dependencies.  
- **Transformer Insights:** Evaluated why Transformers have outperformed RNNs/LSTMs in NLP, and hypothesized that similar advantages (parallelization, attention mechanisms) could improve financial sequence modeling.  
- **Stock Prediction Experiments:** Built standard Transformer networks for predicting closing prices, applied smoothing techniques (moving averages, piecewise regression, bagging), and extended the architecture using multi-head attention to capture inter-stock correlations.  

> Full project description and in-depth results analysis can be found in [Report.pdf](Report.pdf).


---

<details>
<summary><strong>🧠 Neural Networks & Sequence Modeling</strong></summary>

### **Neural Networks**
- Built, trained, and optimized standard feedforward networks.  
- Explored activation functions, loss functions, backpropagation, gradient descent, and regularization methods (dropout, normalization).  

### **Sequence Models**
- **RNNs:** Modeled temporal sequences, but faced vanishing/exploding gradient issues.  
- **LSTMs:** Introduced gating mechanisms to address RNN limitations.  
- **Transformers:** Utilized self-attention and parallelization to model complex dependencies more efficiently than RNNs/LSTMs.  

> Key insight: Transformer architectures offer superior handling of sequential data and longer-term dependencies, suggesting potential for applications beyond NLP.

</details>

---

<details>
<summary><strong>🔧 Transformer Experiments</strong></summary>
  
<br>

- **Standard Transformer:** Designed to predict daily stock closing prices.  
- **Smoothing Techniques:** Applied moving averages, piecewise regression, and bagging to reduce noise and improve prediction stability.  
- **Multi-Head Attention for Correlations:** Captured relationships between stocks, improving robustness of predictions in volatile markets.  

</details>

---

<details>
<summary><strong>📈 Results & Key Findings</strong></summary>

### **Key Results**
- **Short-term prediction difficulty:** High volatility and randomness in stock returns limit the robustness of predictions in short-term windows.  
- **Smoothing improvements:** Techniques like moving averages and piecewise regression improved stability but could not fully overcome inherent market noise.  
- **Correlation modeling with multi-head attention:** Leveraging attention to capture inter-stock correlations significantly improved robustness and reliability of predictions.  
- **Sequence model comparison:** Transformers outperformed RNNs and LSTMs in modeling temporal dependencies, particularly when handling multi-asset interactions.  

### **Limitations**
- Predicting short-term stock returns remains inherently noisy.  
- Out-of-sample generalization is challenging under regime shifts or sudden market changes.  
- No live trading or real-time execution integration; experiments are research-focused.  

### **Planned Improvements**
- Explore hybrid Transformer-LSTM models for enhanced temporal modeling.  
- Integrate additional market features (volume, sector indices, macroeconomic indicators).  
- Extend correlation-based attention modeling to multi-asset portfolios and risk management applications.  

> Overall, while short-term stock return prediction is inherently challenging, attention-based correlation modeling demonstrates a clear improvement in robustness, with promising implications for other time series and multi-variate applications, such as portfolio weight allocation or pairs trading strategies.

</details>

---
