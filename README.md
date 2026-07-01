# 🗾 Tokyo Airbnb Market Analysis & Price Prediction Engine

[![Python](https://img.shields.io/badge/Python-3.8%2B-blue?logo=python&logoColor=white)](https://www.python.org/)
[![Jupyter Notebook](https://img.shields.io/badge/Jupyter-Notebook-orange?logo=jupyter&logoColor=white)](https://jupyter.org/)
[![License](https://img.shields.io/badge/License-MIT-green.svg)](LICENSE)

## 📋 Overview

A comprehensive **Exploratory Data Analysis (EDA)** and **Predictive Pricing Model** for Tokyo's short-term rental market. This project analyzes over **11,000 active Airbnb listings** to identify premium neighborhoods and accurately predict nightly rental prices using machine learning.

> **Key Achievement:** Developed a Random Forest model that reveals the true drivers of Airbnb pricing in Tokyo through feature importance analysis.

---

## 🛠️ Tech Stack

| Component | Technology |
|-----------|-----------|
| **Language** | Python 3.8+ |
| **Data Processing** | Pandas, NumPy |
| **Visualization** | Matplotlib, Seaborn |
| **Machine Learning** | scikit-learn (Random Forest) |
| **Notebook** | Jupyter Notebook |

---

## 🎯 Project Workflow

### 1️⃣ **Data Cleaning & Integrity**
- Filtered high-dimensional dataset to essential commercial metrics
- Processed features: `price`, `minimum_nights`, `number_of_reviews`, `room_type`, `neighbourhood`
- Handled null values and sanitized numerical columns
- Ensured strict data integrity before analysis

### 2️⃣ **Exploratory Data Analysis (EDA)**
- **Market Distribution:** Visualized room type volume and market composition
- **Premium Zone Identification:** Aggregated pricing by neighborhood to identify top 10 most expensive wards
- **Pricing Patterns:** Discovered premium pricing anomalies in specific districts
- **Trend Analysis:** Analyzed relationship between reviews, minimum nights, and pricing

### 3️⃣ **Predictive Modeling**
- **Feature Engineering:** One-Hot Encoding for categorical variables (`room_type`)
- **Model:** Random Forest Regressor trained on property constraints and engagement metrics
- **Evaluation:** Mean Absolute Error (MAE) and R² metrics for model validation
- **Interpretation:** Feature importance analysis to identify key pricing drivers

---

## 💡 Key Business Insights

### What Drives Tokyo Airbnb Prices?

The machine learning model reveals the following feature importance ranking:

| Rank | Feature | Impact | Insight |
|------|---------|--------|---------|
| 🥇 | `minimum_nights` | Highest | Long-term stay constraints dominate pricing strategy |
| 🥈 | `number_of_reviews` | High | Consumer trust & digital reputation drive valuation |
| 🥉 | `room_type` | Moderate | Categorical classification is less influential than operational factors |

**Key Takeaway:** Operational constraints and social proof are far more important than property type in determining Tokyo Airbnb prices.

---

## 📁 Project Structure

```
Tokyo-Airbnb-Market-Analysis/
├── README.md                    # This file
├── *.ipynb                      # Main analysis notebooks
└── data/                        # Dataset files (if included)
```

---

## 🚀 Quick Start

### Prerequisites
```bash
pip install pandas numpy matplotlib seaborn scikit-learn jupyter
```

### Running the Analysis
1. Clone the repository:
   ```bash
   git clone https://github.com/Pysduckrun/Tokyo-Airbnb-Market-Analysis.git
   cd Tokyo-Airbnb-Market-Analysis
   ```

2. Launch Jupyter Notebook:
   ```bash
   jupyter notebook
   ```

3. Open the `.ipynb` file and run cells sequentially to view:
   - Data cleaning pipeline
   - EDA visualizations
   - Model training and evaluation
   - Feature importance analysis

---

## 📊 Analysis Highlights

✅ **Data Size:** 11,000+ active listings  
✅ **Data Quality:** Cleaned and validated across 5+ features  
✅ **Visualizations:** Distribution plots, heatmaps, and feature importance charts  
✅ **Model Performance:** Random Forest with MAE and R² evaluation  
✅ **Business Value:** Actionable insights for pricing strategy  

---

## 🔍 Key Findings

- **Market Composition:** Entire apartments dominate Tokyo's Airbnb market
- **Premium Districts:** Specific wards command significantly higher nightly rates
- **Pricing Drivers:** Minimum night requirements and review counts override room type
- **Prediction Accuracy:** Machine learning model successfully quantifies these relationships

---

## 📈 What You'll Learn

- Modern data cleaning and preparation techniques
- Advanced EDA with Seaborn and Matplotlib
- Feature engineering for machine learning
- Random Forest modeling and hyperparameter tuning
- Interpreting model outputs for business decisions
- Working with real-world marketplace data

---

## 💬 Contact & Contribution

- **Author:** [@Pysduckrun](https://github.com/Pysduckrun)
- **Issues & Suggestions:** Feel free to open an issue!
- **Contributions:** Pull requests are welcome!

---

## 📄 License

This project is licensed under the MIT License - see the LICENSE file for details.

---

<div align="center">

**Made with ❤️ for data enthusiasts and Tokyo market analysts**

[⬆ back to top](#-tokyo-airbnb-market-analysis--price-prediction-engine)

</div>
