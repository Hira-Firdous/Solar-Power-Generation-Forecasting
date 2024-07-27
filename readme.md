# Solar Power Generation Forecasting

This repository contains the implementation of a project focused on forecasting solar power generation using advanced machine learning techniques. 

## Project Overview

The project aims to enhance the accuracy of short-term solar power generation predictions by utilizing a dataset containing historical solar power generation data and various meteorological parameters. Accurate forecasting is crucial for optimizing energy production, distribution, and resource utilization, which ultimately contributes to efficient grid management and improved sustainability.

### Key Objectives
- **Model Implementation**: Develop and implement neural network models for accurate solar power forecasting.
- **Data Understanding**: Analyze correlations between different meteorological and environmental factors affecting solar power generation.
- **Model Evaluation**: Use evaluation metrics like Root Mean Square Error (RMSE) and Coefficient of Determination (R²) to assess model performance.

## Dataset

The dataset utilized in this project is sourced from [GitHub](https://github.com/anantgupta129/Solar-Power-Generation-Forecasting/tree/main). It includes a comprehensive set of features, such as:

- Distance-to-solar-noon
- Daily average temperature
- Daily average wind direction and speed
- Sky cover (scale of 0-4)
- Visibility
- Humidity
- Power generated in joules for each 3-hour period

The data is collected from various sources, including solar farms, weather stations, and environmental databases.

## Methodology

### Data Understanding
The data was analyzed to understand the relationships and correlations between different parameters. A heatmap was generated to visualize these correlations, revealing important patterns such as:

- High correlation between Zenith and Angle of Incidence (0.71)
- Negative correlation between Zenith and temperature (-0.55)
- Positive correlation between Relative Humidity and Low Cloud Cover (0.49)

### Model Implementation
The model used is a simple Artificial Neural Network (ANN) with the following structure:
- Two hidden layers with 32 and 64 neurons, respectively
- The model predicts the total power generated based on 19 input parameters

### Evaluation Metrics
The model's performance was evaluated using:
- **Root Mean Square Error (RMSE)**: Indicates the standard deviation of prediction errors.
- **Coefficient of Determination (R²)**: Measures the proportion of variance in the dependent variable that is predictable from the independent variables.

## Results and Findings

- **RMSE**: The model showed a significant reduction in error towards the end of the training epochs.
- **R² Score**: The model's R² score indicates its effectiveness in fitting the data, providing a good measure of prediction accuracy.

## Future Work

### Proposed Enhancements
- **Automation with IoT**: Future work includes automating the data collection process using IoT devices. This approach would involve embedding sensors and IoT devices to continuously feed real-time data into the model, enabling more accurate and timely predictions.

## References

1. [Power output forecasting of solar photovoltaic plant using LSTM](https://doi.org/10.1016/j.geits.2023.100113)
2. [Solar-Power-Forecasting Master Thesis](https://github.com/saradindusengupta/Solar-Power-Forecasting/blob/master/Master%20Thesis.pdf)
3. [Solar-Power-Generation-Forecasting Dataset](https://github.com/anantgupta129/Solar-Power-Generation-Forecasting/blob/main/solarpowergeneration.csv)
4. [Analysis of Factors for Forecasting Electric Power Generation by Solar Power Plants](https://ela.kpi.ua/bitstream/123456789/54368/1/eete2020-4_62_p64-69.pdf)
5. Ashraf, I., & Chandra, A. "Artificial neural network based models for forecasting electricity generation of grid connected solar PV power plant," International Journal of Global Energy Issues, vol. 21, no. 1/2, p. 119, Jan. 2004.

## Installation and Usage

### Prerequisites
- Python 3.x
- Required libraries: numpy, pandas, sklearn, matplotlib, etc.

### Installation
Clone this repository and install the required dependencies:

```bash
git clone https://github.com/anantgupta129/Solar-Power-Generation-Forecasting.git
cd Solar-Power-Generation-Forecasting
