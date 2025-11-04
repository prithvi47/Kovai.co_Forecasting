# Kovai.co_Forecasting

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
