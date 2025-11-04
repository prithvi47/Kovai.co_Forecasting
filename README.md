# Kovai.co_Forecasting
# 🧭 Public Transport Ridership Forecasting — EDA & Insights Report

## 📌 Objective

This project focuses on analyzing and forecasting public transport ridership data across multiple service types such as **Local Route**, **Light Rail**, **Peak Service**, **Rapid Route**, and **School Services**.
The goal is to uncover **seasonality, trends, and outliers**, and to predict short-term ridership demand for operational optimization.

---

## 🧹 Step 1: Exploratory Data Analysis (EDA)

### 🔹 Data Cleaning

* Removed missing or duplicate values.
* Ensured all timestamps were converted to `datetime` format.
* Verified consistent service columns across datasets.
* Aggregated data at a daily level for trend analysis.

### 🔹 Trend and Seasonality Exploration

* Identified strong weekday peaks for *Local* and *Peak* routes.
* *Light Rail* showed steady post-pandemic recovery and weekend stability.
* *School* routes were active only on weekdays.
* Seasonal trend analysis revealed cyclic patterns matching commuting hours.

### 🔹 Outlier Detection

* Used boxplots and rolling means to detect abnormal ridership spikes (e.g., festival events, strikes).
* Outliers were retained when corresponding to real-world events.

---

## 🔮 Step 2: Forecasting

A **Random Forest Regressor** model was used for short-term (7-day) forecasts.
Each service’s historical ridership was modeled separately to predict future trends.

### 🧩 Model Evaluation Metrics

| Metric | Description                       | Typical Range |
| ------ | --------------------------------- | ------------- |
| MAE    | Measures average prediction error | 8,000–10,000  |
| RMSE   | Penalizes large errors            | 9,000–12,000  |
| R²     | Goodness of fit                   | 0.79–0.88     |

---

## 📊 Step 3: Visualizations

1. **📈 Historical vs Forecast Trends** – Past 90 days vs 7-day predictions.
2. **🚍 Multi-service Trends** – Comparative ridership trajectories across routes.
3. **📆 Weekly Seasonality** – Clear weekday patterns in commuter traffic.
4. **🎯 Model Performance Dashboard** – MAE, RMSE, and R² visualized side-by-side.
5. **🧭 Insight Summary Table** – Concise, actionable takeaways.

---

## 💡 Step 4: Insights and Recommendations

| Category               | Key Observation                   | Recommended Action                              |
| ---------------------- | --------------------------------- | ----------------------------------------------- |
| 🚀 Local & Peak Routes | Strong weekday peaks              | Optimize weekday scheduling                     |
| 🚈 Light Rail          | Steady growth                     | Promote usage & schedule preventive maintenance |
| 🏫 School Services     | Stable weekday pattern            | Adjust fleet size for school hours              |
| ⚡ Rapid Route          | Rising trend                      | Increase frequency during rush hours            |
| 📊 Forecast (7-day)    | 5–10% ridership increase expected | Prepare for higher operational load             |

---

## 🧠 Conclusion

The analysis provides actionable insights into **ridership demand patterns**, enabling transport authorities to:

* Allocate resources efficiently.
* Plan maintenance without service disruptions.
* Prepare for short-term increases in demand.
  This project demonstrates the synergy between **data science** and **urban mobility optimization**.

---

## ⚙️ Tech Stack

* **Python**, **Google Colab**
* **Pandas**, **Matplotlib**, **Seaborn**, **Scikit-learn**
* **Random Forest Regressor**
* **Time Series Forecasting** & **EDA Visualization**

---

## 📂 Files

| File                             | Description                                                     |
| -------------------------------- | --------------------------------------------------------------- |
| `Untitled27.ipynb`               | Complete Colab notebook for data cleaning, EDA, and forecasting |
| `forecast_insight_dashboard.png` | Visualization summary (optional export)                         |
| `REPORT.md`                      | Detailed project report                                         |
| `README.md`                      | GitHub project overview                                         |

Overview
This repository contains the code and visualizations for public transport ridership forecasting using time series and machine learning techniques. It provides Exploratory Data Analysis (EDA), forecast visualization, and insight dashboards to assist transit planners in data-driven decision-making.

📊 Key Features
* Data cleaning and preprocessing for ridership datasets
* Time series analysis for multiple transport services
* Short-term ridership forecasting using Random Forest
* Weekly seasonality and trend visualization
* Interactive insight dashboard with performance metrics and recommendations

🧠 Technologies Used
* Language: Python
* Environment: Google Colab
* Libraries: Pandas, NumPy, Matplotlib, Seaborn, Scikit-learn

🧭 Workflow
1. Load & Clean Data
    * Convert timestamps to datetime
    * Remove duplicates and handle nulls
2. Perform EDA
    * Explore daily and weekly patterns
    * Visualize seasonality and anomalies
3. Train Forecasting Model
    * Apply Random Forest Regressor
    * Evaluate using MAE, RMSE, R²
4. Generate Dashboard
    * Compare historical vs forecasted ridership
    * Display weekly seasonality
    * Summarize insights in tables and charts

📈 Sample Insights
Service	Insight	Recommendation
Local Route	Weekday peak demand	Add more buses during morning/evening
Light Rail	Gradual growth	Continue expansion & promotion
Rapid Route	Upward trend	Increase capacity during rush hours

📂 Repository Structure
├── Untitled27.ipynb          
├── REPORT.md                 
├── README.md                 
└── data/                     

🚀 How to Run
1. Clone this repository  git clone
2. cd public-transport-forecast
3. Open forecating.ipynb in Google Colab
4. Run all cells sequentially
5. View final visualization dashboards and insights
