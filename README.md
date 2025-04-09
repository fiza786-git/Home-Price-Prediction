# US Home Price Analysis 

The goal is to analyze publicly available economic factors and explain how they have influenced **US home prices** over the past 20 years.

---

## 📊 Problem Statement
To build a data science model that explains how various macroeconomic and financial factors have impacted U.S. home prices over the last 20 years, using the S&P Case-Shiller Home Price Index as a proxy.


---

## 📁 Data Sources

All datasets were obtained from [FRED - Federal Reserve Economic Data](https://fred.stlouisfed.org/):

| Dataset               | FRED Series Code    | Description                              |
|----------------------|---------------------|------------------------------------------|
| Home Price Index     | `CSUSHPISA`         | National home prices (Case-Shiller Index)|
| Unemployment Rate    | `UNRATE`            | National unemployment rate (%)           |
| CPI (Inflation)      | `CPIAUCNS`          | Consumer Price Index (CPI-U)             |
| Housing Starts       | `HOUST`             | New privately-owned housing starts       |
| Fed Funds Rate       | `FEDFUNDS`          | Federal interest rate                    |
| Median Household Income | `MEHOINUSA672N` | Median household income in the US        |
| MORTGAGE30US.csv        | MortgageRate     | 30-Year Fixed Rate Mortgage Average in the U.S.|

---

## 🛠️ Methods Used

- Data Wrangling & Preprocessing (handling missing values, scaling, feature engineering)
- Assumption checks (normality, multicollinearity using VIF, linearity)
- Exploratory Data Analysis (EDA)
- Regression & Tree-Based Models
- Model Evaluation (R², MAE)

---

## 📈 Model Performance

**Final Model Used:** Gradient Boosting Regressor  
- **Train R²**: 0.999  
- **Test R²**: 0.997  
- **MAE**: ~0.0157  
Model showed high performance and generalization across the 20-year dataset.

---

## 🔍 Key Insights

- Inflation (CPI) and Fed Funds Rate are strongly associated with changes in home prices.
- Tree-based models handled non-linear relationships better than linear regression.
- Feature engineering and lag-based features significantly improved model performance.
- Home prices have seen a sharp rise post-2020, influenced by low interest rates and inflation.

---
## 📁 Project Structure

project-root/
│
├── CPIAUCNS.csv           # Consumer Price Index
├── CSUSHPISA.csv          # S&P/Case-Shiller U.S. National Home Price Index
├── FEDFUNDS.csv           # Federal Funds Rate
├── HOUST.csv              # Housing Starts Data
├── MEHOINUSA672N.csv      # Median Household Income
├── MORTGAGE30US.csv       # 30-Year Fixed Mortgage Rate
├── UNRATE.csv             # Unemployment Rate
│
├── Home_Price_Prediction.ipynb   # Main notebook with full analysis and modeling
├── README.md                     # Project documentation
            



