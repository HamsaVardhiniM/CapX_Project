# CapX_Project

# Stock Price Prediction Using Sentiment Analysis and Time Series  

This project integrates sentiment analysis of social media posts with **time-series analysis** of historical stock prices to predict stock prices with improved accuracy. The final predictions combine the strengths of both models: ARIMA for capturing trends in historical data and a Ridge Regression-based sentiment model for incorporating additional influencing factors like sentiment scores.

---

## Project Overview  
1. **Data Sources**:  
   - Reddit posts (past 2 years) scraped using the Reddit API.  
   - Historical stock prices fetched using the `yfinance` library for stocks: **AAPL, MSFT, TSLA, GOOGL, AMZN**.  

2. **Key Models**:  
   - **ARIMA**: Forecasts stock prices by analyzing historical trends.  
   - **Sentiment-Based Model**: Incorporates sentiment scores, topics, stock types, and other features extracted from Reddit posts.  

3. **Integration**:  
   The results of both models are combined with weight optimization for better accuracy.  

---

## Key Features  
1. **Sentiment Analysis**: Analyzes sentiment polarity, subjectivity, and topics from Reddit posts.  
2. **ANOVA Testing**: Identifies stock type as a significant factor influencing stock price.  
3. **Feature Engineering**: Extracts meaningful features like weekday, month, sentiment scores, and volume for model training.  
4. **Error Optimization**: Combines predictions from ARIMA and Ridge Regression using weighted averaging based on model performance.  

---

## Project Workflow  
The project is structured into **7 phases**, each encapsulated in a Jupyter notebook:  
1. **Data Collection**: Scrapes Reddit posts and fetches historical stock prices.  
2. **Sentiment Analysis & Merging**: Performs sentiment analysis and integrates data into a single dataset.  
3. **EDA & ANOVA Testing**: Explores data trends and derives insights about feature relevance.  
4. **Feature Engineering**: Preprocesses and enriches data with additional attributes.  
5. **ARIMA Model**: Predicts stock prices based on historical data with minimal error.  
6. **Sentiment Model**: Trains machine learning models using all features, achieving high accuracy.  
7. **Combining Results**: Optimizes weights to integrate predictions from both models.  

---

## Tools Used  
- **Python Libraries**: `yfinance`, `pandas`, `scikit-learn`, `statsmodels`, `NLTK`  
- **APIs**: Reddit API for data scraping  
- **ML Techniques**: Ridge Regression, ARIMA, Sentiment Analysis  
- **Jupyter Notebooks**: Organized workflow  

---

## How to Use  
1. Clone the repository.  
2. Run Jupyter notebooks in sequence for full pipeline execution.  
3. Use `requirements.txt` for installing dependencies.
4. Or just download the notebooks directly and run them locally

---

## Repository Structure  
- Notebooks: 7 notebooks for each phase of the project.  
- Data: Merged datasets (`.csv`).  
- Configuration: Setup and requirements files for easy execution.  

---

## Improvements & Future Work  
1. Expand data sources to include Twitter and financial news.  
2. Incorporate more advanced models like LSTM for time series.  
3. Analyze global events impacting stock prices.  
4. Enhance sentiment analysis with contextual embeddings (e.g., BERT).  

---

## Links  
- **GitHub Repository**: [Insert Link]  
- **Demo Video**: [Insert Link]  



