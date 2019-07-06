---
layout: page
feature_image: "https://picsum.photos/1300/400?image=989"
feature_text: |
  ## COMP7704 Computing Projects in Algo Finance
  ## (Trading Strategy of Strategies)
  ## 
  ## CHAN Yiu Keung (2011565354)
  ## Supervisor: Dr. Hilton K.H. Chan
---


### Abstract
This study tries to make use of arbitrary features (aka: signals or columns) to predict future price change in Foreign Exchange Market (Forex). In particular, technical indicators (eg: MACD, RSI etc) and pattern analysis are introduced as the features of each timestep. To make use of multiple features, a composite neural network (Bi-LSTM + BERT) is trained and evaluated on 4 different currency pairs (USDCAD, USDJPY, AUDUSD, EURUSD) separately.

---

### Objectives
* Make use of arbitrary features (aka: signals) to predict future price change in Forex market
* Generate signals using technical indicators and candle pattern analysis
* Select a subset of relatively important features for training machine learning model
* Apply a composite neural network (Bi-LSTM + BERT) for predicting future price movement
