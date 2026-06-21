# Supermarket Sales Data Analysis & Performance Drivers

## 📌 Project Overview
This project performs an end-to-end Exploratory Data Analysis (EDA) on a dataset of 14,204 supermarket transactions. The goal is to identify the core product and outlet characteristics that drive the highest revenue, providing data-backed recommendations for inventory optimization and expansion strategy. 

## 🛠️ Tech Stack & Tools
* **Language:** Python
* **Libraries:** Pandas (Data Manipulation), Matplotlib & Seaborn (Data Visualization)
* **Environment:** Jupyter Notebook
* **Key Concepts:** Data Imputation, Statistical Correlation, Linear Regression
  
## 🧹 Data Cleaning & Preprocessing
To ensure analytical validity, the dataset underwent rigorous cleaning:
* **Imputation:** Filled 2,439 missing `Item_Weight` values using the column Mean, and 4,016 missing `Outlet_Size` values using the Mode.
* **Standardization:** Corrected inconsistent cashier data entry in the Fat Content column (merging "LF", "low fat", and "reg" into standard categories).
* **Anomaly Detection:** Flagged 879 items registered with exactly 0.0% shelf visibility for operational review.

## 📊 Key Insights & Visualizations
1. **Price is the Strongest Driver (r = 0.60):** A statistical correlation matrix and linear regression scatter plots proved that Item Price (MRP) has a strong positive correlation with Total Sales. Physical item weight (r = 0.02) has zero impact on purchasing behavior.
2. **The Flagship Format:** Supermarket Type 1 is the undeniable core business, generating 69.3% of total company revenue ($20.6M).
3. **Geographic Efficiency:** Contrary to conventional assumptions, Tier 3 locations generate the highest total volume ($12.3M), significantly outperforming Tier 1 cities ($7.1M). Medium-sized stores also outperformed High-capacity stores.
4. **The 1998 Anomaly:** Time-series analysis revealed a massive operational drop for stores established in 1998, where average sales plummeted to just $323, warranting further investigation.

## 💡 Strategic Business Recommendations
To maximize ROI, marketing and expansion budgets should be heavily weighted toward stocking higher-MRP items specifically inside Tier 3, Supermarket Type 1 locations—the highest-efficiency intersection of store format and geography identified in this analysis.
