# Home Energy Consumption Prediction Based on Smart Meter Data
![Diagram](images/hero.png)
## Overview
This project aims to create a predictive model for household energy consumption using historical data from smart meters and external factors such as weather conditions. \
By leveraging the UCI Household Power Consumption Dataset and weather data from the Meteostat API, the model seeks to provide insights into energy usage patterns and assist in optimizing consumption.

## Dataset Information
- **Energy Consumption Dataset**: [UCI Household Power Consumption Dataset](https://archive.ics.uci.edu/dataset/235/individual+household+electric+power+consumption)
  - Contains measurements of household energy consumption between December 2006 and November 2010.
- **Weather Data**: Collected from the Meteostat API, including temperature, precipitation, and other weather variables.

### Key Features
- **Energy Dataset Features**:
  - Date, Time, Global Active Power, Global Reactive Power, Voltage, Global Intensity, Sub-metering data.
  
- **Weather Dataset Features**:
  - Average Temperature, Minimum and Maximum Temperature, Total Precipitation, Snow Depth, Wind Speed, Sea-Level Pressure.

## Requirements
- Python 3.x
- Libraries: `numpy`, `pandas`, `matplotlib`, `seaborn`, `sklearn`, `ydata_profiling`, `meteostat`

## Data Preprocessing
1. **Cleaning**: Handling missing values and formatting datetime.
2. **Feature Engineering**: Creating lag features, interaction features, and seasonal indicators.
3. **Merging Datasets**: Combining energy and weather datasets based on datetime.

## Model Training and Evaluation
- **Model Used**: Linear Regression
- **Evaluation Metrics**: RMSE, MAE, R-squared
- The model achieved a high R-squared value of 99.86%, indicating excellent predictive accuracy.

## Data Visualization
Visualizations include:
- Time series plots of global active power.
- Distribution analysis of energy consumption.
- Correlation heatmaps and seasonal consumption trends.

**For viewing the profiling of data use the link:** \
[Household Energy Consumption Profile Report](https://snehapadgaonkar.github.io/Household-energy-consumption-prediction/household_consumption_profile_report.html)

## Future Scope
1. **Integration with IoT Devices**: Expand the model to capture real-time data from smart home devices to improve accuracy and optimization of energy use.
2. **Predictive Maintenance**: Identify patterns that signal potential equipment failures, enabling proactive maintenance to enhance efficiency.

## Usage
1. Clone the repository:
   ```bash
   git clone https://github.com/snehapadgaonkar/Household-energy-consumption-prediction.git
   cd final
2. Load the Dataset: Ensure you have the dataset in the specified location or update the path in the notebook.
3. Install the required libraries:
   ```bash
   pip install -r requirements.txt
4. Run the Notebook: Open the Jupyter Notebook and follow the steps for data preprocessing, feature engineering, and model evaluation.

## Conclusion
This project effectively utilizes machine learning to forecast household energy usage, achieving high accuracy with a 99.86% R-squared value. \
By integrating historical data and weather factors, it provides actionable insights for optimizing energy consumption.