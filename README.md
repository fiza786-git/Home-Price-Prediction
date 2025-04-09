# US Home Price Analysis (2004–2024)

This project is part of the Stage 1 interview with **Home.LLC** for the **Quantitative Analytics** team.  
The goal is to analyze publicly available economic factors and explain how they have influenced **US home prices** over the past 20 years.

---

## 📊 Problem Statement

> Build a data science model that explains how publicly available factors have impacted US home prices nationally from 2004 to 2024.  
> Use the **S&P Case-Schiller Home Price Index** as a proxy for home prices.

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

## 📂 File Structure
home-price-analysis/ ├── Home_Price_Analysis.ipynb # Main notebook ├── data/ └── README.md



