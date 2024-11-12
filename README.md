# Walmart Store Sales Forecasting

This repository contains a time series forecasting project on Walmart store sales data, using machine learning techniques to predict demand and account for seasonal events. The objective is to accurately model sales trends, identify anomalies, and build regression models to understand how various factors affect sales across multiple Walmart stores in the U.S.

## Table of Contents
- [About the Dataset](#about-the-dataset)
- [Project Objectives](#project-objectives)
- [Project Structure](#project-structure)
- [Installation](#installation)
- [Usage](#usage)
- [Results](#results)
- [License](#license)

---

## About the Dataset
This dataset, sourced from world.data, provides historical sales information for 45 Walmart stores in different regions. The data includes weekly sales figures, promotional markdown events, and economic indicators (CPI, Unemployment Index). The data also captures sales influences due to major U.S. holidays, like the Super Bowl, Labour Day, Thanksgiving, and Christmas. These holiday weeks are given extra weighting due to their impact on sales patterns.

**Key Features**:
- **Sales**: Weekly sales figures for each store.
- **Holiday Events**: Sales during major holidays with increased evaluation weighting.
- **Economic Indicators**: Factors like CPI and Unemployment Index that may affect sales.
- **Promotional Events**: Walmart markdowns scheduled around holidays.

## Project Objectives
1. **Data Exploration**: Analyze and understand the structure and characteristics of the dataset.
2. **Time Series Forecasting**: Develop time series models to predict sales over time and assess trends.
3. **Anomaly Detection**: Identify irregular patterns or anomalies in sales data.
4. **Regression Analysis**: Build regression models to predict sales based on features such as economic indicators and promotions.
5. **Model Evaluation**: Evaluate models using metrics such as R², RMSE, and others to understand prediction accuracy and model performance.

## Project Structure
The repository is organized as follows:


## Installation

1. Clone this repository:
   ```bash```
   git clone https://github.com/yourusername/time-series-forecasting-stock-sales.git
   cd time-series-forecasting-stock-sales.

2. Create and activate a virtual environment
   python3 -m venv venv
  source venv/bin/activate       # For macOS/Linux
  source venv\Scripts\activate          # For Windows
3. Install the required packages
   pip install -r requirements.txt

# Usage
- Data Preprocessing

Load and preprocess data for analysis. Use notebooks/EDA.ipynb for initial data exploration and cleaning.
Save cleaned data to data/cleaned_data.csv.
- Modeling

Use notebooks/modeling.ipynb to build and evaluate time series and regression models.
Tried different models like SARIMA, Prophet, and regression models, and compare their performance on the test set.
- Anomaly Detection

Identify and analyze any irregular patterns in sales data, particularly around holidays and promotions.

- Evaluation

Evaluate model performance using metrics like R² and RMSE.
Document insights in the notebooks/modeling.ipynb notebook and include visualizations.

- Results
The project results include:

Predicted sales trends over time.
Impact of holidays, economic factors, and markdown events on Walmart sales.
Comparison of model performance using R² and RMSE metrics.
Results are documented in the notebooks, including visualizations and explanations of the findings.

- License
This project is licensed under the MIT License - see the LICENSE file for details.

