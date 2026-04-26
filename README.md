#  Stock Price Prediction (Short-Term) — Research-Based Project

## 📌 Overview

This project focuses on predicting the **next day’s closing stock price** using historical market data. A research-oriented approach is applied to explore relationships between stock features and evaluate machine learning models for short-term forecasting.

The analysis combines **data exploration, regression modeling, and visualization** to derive meaningful insights about stock price behavior.


## 🎯 Objectives

- Analyze historical stock market data  
- Understand relationships between price features  
- Build predictive models for short-term forecasting  
- Compare performance of linear and non-linear models  
- Evaluate predictions using metrics and visualization  


## 📊 Dataset

- **Source:** Yahoo Finance (via `yfinance` API)  
- **Stock Used:** Apple (AAPL) *(can be changed)*  
- **Time Period:** Last 2 years (daily data)  

### Features Used:
- Open  
- High  
- Low  
- Volume  

### Target:
- Close (Next Day Closing Price)


## 🔍 Methodology

### 1. Data Collection
- Retrieved stock data using `yfinance`

### 2. Data Exploration
- Checked structure, statistics, and consistency  
- Verified absence of major missing values  

### 3. Feature Selection
- Selected price-based and volume features  

### 4. Model Training
- **Linear Regression** (baseline model)  
- **Random Forest Regressor** (non-linear model)  

### 5. Evaluation Metrics
- Mean Squared Error (MSE)  
- R² Score  

### 6. Visualization
- Compared actual vs predicted prices using line plots  


## 🧠 Model Performance

| Model              | MSE ↓ | R² ↑ | Performance |
|-------------------|------|------|------------|
| Linear Regression | 2.45 | 0.975 |  Excellent |
| Random Forest     | 9.81 | 0.902 |  Moderate |


## 📊 Key Findings

- Linear Regression outperformed Random Forest in both accuracy and visualization  
- Strong linear relationship exists between:
  - Open, High, Low → Close price  
- Random Forest showed larger deviations and lower generalization performance  


## ⚙️ Important Insight

Although stock markets are often considered complex and non-linear, this study shows that:

> **Short-term stock price prediction can be effectively modeled using simple linear relationships when features are highly correlated.**

This highlights the importance of **understanding data before choosing complex models**.


## ⚠️ Limitations

- External factors (news, economy, sentiment) not included  
- No technical indicators used (e.g., moving averages)  
- Limited to short-term prediction  
- Models not hyperparameter-tuned  

## 🚀 Future Work

- Add lag features (previous day prices)   
- Apply advanced models (LSTM, XGBoost)  
- Integrate sentiment analysis from news/social media  
- Deploy a real-time prediction system  


## 🏁 Conclusion
This project demonstrates that **model simplicity can outperform complexity** when data relationships are inherently linear.

Linear Regression proved to be highly effective for short-term stock prediction, while Random Forest did not provide additional benefits without tuning.

> **The key takeaway:**  
> Choosing the right model depends more on **data characteristics** than model complexity.

## 📁 Project Structure
Predict_Future_Stock_Prices/
│── stock_prediction.ipynb
│── README.md

## 🛠️ Tools & Libraries

- Python  
- Pandas  
- Matplotlib  
- Seaborn  
- Scikit-learn  
- yfinance  

## 👨‍💻 Author

**Malik Muhammad Mudassir Iqbal**  
AI/ML Engineering Intern — DevelopersHub Corporation