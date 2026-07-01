# Tokyo Airbnb Market Analysis & Price Prediction Engine

## Overview
This project explores the Tokyo short-term rental market to identify premium real estate zones and predict property pricing. Utilizing a dataset of over 11,000 active listings, the project moves from exploratory data analysis (EDA) to deploying a supervised machine learning model that extracts the primary drivers of market valuation.

## Tech Stack
* **Language:** Python
* **Data Processing:** Pandas, NumPy
* **Visualization:** Matplotlib, Seaborn
* **Machine Learning:** scikit-learn (Random Forest Regressor)

## Project Workflow

### 1. Data Cleaning & Integrity
* Filtered a high-dimensional dataset down to essential commercial metrics (`price`, `minimum_nights`, `number_of_reviews`, `room_type`, `neighbourhood`).
* Handled null values and sanitized numerical columns to ensure strict data integrity before analysis.

### 2. Exploratory Data Analysis (EDA)
* **Market Distribution:** Visualized the volume of room types, revealing a heavy market skew toward entire apartments over shared or private rooms.
* **Premium Real Estate Identification:** Aggregated pricing by neighborhood to identify the top 10 most expensive wards. Uncovered premium pricing anomalies in rural retreat districts (e.g., Okutama-machi) compared to high-volume central Tokyo wards.

### 3. Predictive Modeling
* Engineered categorical features using One-Hot Encoding to prepare textual data (`room_type`) for the machine learning pipeline.
* Built and trained a **Random Forest Regressor** to predict nightly listing prices based on property constraints and historical engagement. 
* Evaluated model accuracy using Mean Absolute Error (MAE) and R-squared metrics.

## Key Business Insights
The machine learning model's feature importance extraction provided data-backed answers on what truly drives Airbnb prices in Tokyo:
* **Operational Constraints Dominate:** The `minimum_nights` requirement is the most critical feature driving price predictions in the Tokyo market[cite: 1]. This indicates that long-term stays operate on a fundamentally different commercial pricing tier than nightly tourist rentals.
* **Social Proof is Valuation:** The `number_of_reviews` is the second most important predictive feature[cite: 1]. In digital hospitality marketplaces, accumulated consumer trust and digital reputation directly correlate with a property's financial valuation. 
* **Room Type is Secondary:** Categorical classifications (like private rooms vs. shared rooms) proved far less influential on the final price than duration constraints and review volume[cite: 1].

## How to Run
1. Clone the repository to your local machine.
2. Ensure you have the required libraries installed (`pip install pandas numpy matplotlib seaborn scikit-learn`).
3. Run the Jupyter Notebook (`.ipynb` file) cell by cell to view the data pipeline, visual charts, and model outputs.
