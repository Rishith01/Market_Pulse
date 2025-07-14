# Market_Pulse

# 📈 Market Pulse: Stock Trend Prediction Using Multivariate LSTM and Sentiment Analysis

This project was developed as part of the **WIDS 4-Week Project**, focusing on forecasting stock trends by combining **time series modeling** and **natural language sentiment analysis**. The weekly structure covered the foundations of stock prediction, classic statistical methods like ARIMA, and advanced models like LSTMs, culminating in a final hybrid model using **LSTM + sentiment polarity**.

---

## 🗓️ Weekly Breakdown

### 📌 Week 0: Time Series & Python Fundamentals

- Learned basics of time series forecasting using Python.
- Used `yfinance` to fetch 5 years of NASDAQ data.
- Performed EDA: plotted price trends, moving averages, and trading volume.
- Observed noise in volume vs. smoother trends in price data.

### 📌 Week 1: Sentiment Analysis on Text Data

- Introduced to NLP using `TextBlob`.
- Preprocessed text (IMDb Netflix dataset) — cleaned, lemmatized, removed special chars.
- Extracted **polarity** and **subjectivity** scores.
- Built sentiment analysis foundation to later apply to financial news.

### 📌 Week 2: Reinforcement Learning & ARIMA Modeling

- Brief intro to RL concepts.
- Implemented **ARIMA** model for stock prediction using grid search for best `(p,d,q)` values.
- Used MAE, MSE, RMSE for evaluation.
- Learned limitations of ARIMA in capturing long-term trends.

### 📌 Week 3: Univariate LSTM vs. ARIMA

- Built a basic **LSTM** for univariate stock data.
- Compared ARIMA and LSTM predictions.
- LSTM showed better ability to model nonlinear trends but required hyperparameter tuning.
- Gained intuition on how sequential deep models outperform statistical ones for complex time series.

---

## 🧠 Week 4: Final Project — LSTM + Sentiment

### Goal:
Predict Tesla stock price by combining:
- Historical price and volume data
- Sentiment polarity from financial news (Kaggle dataset)

### Approach:
- Appended news sentiment polarity to price dataset.
- Preprocessed news and extracted **only polarity**.
- Trained **multivariate LSTM** using both price and sentiment.
- Evaluated results on training, validation, and test sets.

### Observations:
- LSTM captured price trends better than ARIMA.
- Predictions often underestimated actual prices.
- Sentiment signals were sparse, possibly limiting model strength.
- News had impact, but better real-time or richer sentiment sources could improve accuracy.

---

## 🔬 Key Learnings

- Time series requires careful preprocessing and trend understanding.
- Sentiment adds interpretability to price movements.
- LSTM models are powerful but sensitive to data quality and size.
- Combining **structured (price)** and **unstructured (text)** data is challenging but promising.

---

## 🚀 Future Work

- Use real-time news feeds or social media sentiment (Twitter, Reddit).
- Explore transformer-based models (e.g., BERT) for sentiment.
- Add attention mechanisms to LSTM.
- Try ensemble models combining LSTM, ARIMA, and sentiment separately.

