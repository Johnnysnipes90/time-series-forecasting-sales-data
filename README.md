# Walmart Store Sales Forecasting

This repository contains a time series forecasting project on Walmart store sales data. We aim to predict demand, account for seasonal events, and evaluate machine learning models to improve forecast accuracy for Walmart sales across 45 stores in the U.S.

## Table of Contents
- [About the Dataset](#about-the-dataset)
- [Data Dictionary](#data-dictionary)
- [Project Objectives](#project-objectives)
- [Project Structure](#project-structure)
- [Installation](#installation)
- [Usage](#usage)
- [Results](#results)
- [License](#license)

---

## About the Dataset
The Walmart sales dataset provides historical data for 45 Walmart stores located in different regions, with information on weekly sales, holiday indicators, promotional markdowns, and economic conditions like the Consumer Price Index (CPI) and Unemployment Index. Major U.S. holidays, such as the Super Bowl, Labour Day, Thanksgiving, and Christmas, are given special weighting due to their impact on consumer demand.

The dataset aims to capture factors that drive sales variations across different departments, store locations, and holiday periods, providing a robust base for sales forecasting and regression modeling.

**Source**: The dataset is sourced from world.data.

## Data Dictionary
Here's a brief description of each column in the dataset:

| Column         | Description                                                                 |
|----------------|-----------------------------------------------------------------------------|
| `Unnamed: 0`   | Row index (may be removed in preprocessing).                               |
| `Store`        | Store ID (unique identifier for each store).                               |
| `Date`         | The date for the weekly sales data.                                        |
| `IsHoliday`    | Indicator (1 = holiday week, 0 = non-holiday week).                        |
| `Dept`         | Department ID (unique identifier for each department within the store).    |
| `Weekly_Sales` | Sales revenue for the given week in the respective department.             |
| `Temperature`  | Average temperature for the week at the store's location.                  |
| `Fuel_Price`   | Fuel price at the store's location (may influence purchasing patterns).    |
| `MarkDown1-5`  | Data on promotional markdowns preceding major holidays (when available).   |
| `CPI`          | Consumer Price Index (economic indicator, affects purchasing power).       |
| `Unemployment` | Unemployment rate at the store's location (affects local spending habits). |
| `Type`         | Store type classification (categorical).                                   |
| `Size`         | Store size in square feet.                                                 |

## Project Objectives
1. **Data Exploration**: Analyze and understand the structure and characteristics of the dataset.
2. **Time Series Forecasting**: Develop time series models to predict weekly sales.
3. **Anomaly Detection**: Identify unusual sales patterns, particularly around holidays and markdown events.
4. **Regression Analysis**: Build regression models to predict sales based on economic indicators and store-specific data.
5. **Model Evaluation**: Compare model performance with metrics like R², RMSE, etc.

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

