# Prediction of Carbon Monoxide (CO) Levels Using Machine Learning

This project is a part of the AAI-550 course in the Applied Artificial Intelligence Program at the University of San Diego (USD).

## Project Status: Completed

## Installation

### Prerequisites
- Python 3.7 or higher
- Git
- Jupyter Notebook or JupyterLab or Google Colab (optional, for running notebooks)

### Steps
1. Clone the repository:
   ```
   git clone https://github.com/karthikmekala12343/uci-ml-prediction-of-co-levels.git
   cd uci-ml-prediction-of-co-levels
   ```

2. Install required Python packages:
   ```
   pip install pandas numpy scikit-learn matplotlib seaborn statsmodels ucimlrepo jupyter
   ```
   Or if a `requirements.txt` file is present:
   ```
   pip install -r requirements.txt
   ```

3. Launch Jupyter Notebook:
   ```
   jupyter notebook
   ```
   Or for JupyterLab:
   ```
   jupyter lab
   ```

4. Open and run the notebooks: `Prediction_of_CO_Levels_Using_Machine_Learning.ipynb` to explore the analysis.

### Using Google Colab
If you prefer a cloud-based environment without local setup:

1. Go to [Google Colab](https://colab.research.google.com/)

2. Open the notebooks from the GitHub repository:
   - Navigate to https://github.com/karthikmekala12343/uci-ml-prediction-of-co-levels
   - Click on the `.ipynb` files and select "Open in Colab"

3. In the first cell, install dependencies:
   ```
   !pip install -r https://raw.githubusercontent.com/karthikmekala12343/uci-ml-prediction-of-co-levels/main/requirements.txt
   ```

4. Run the notebook cells.

### Notes
- The project uses the UCI Air Quality dataset, which is automatically fetched in the code using the `ucimlrepo` package.
- Ensure you have a stable internet connection for dataset download if not cached locally.

## Project Intro/Objective

The main purpose of this project is to analyze air quality data from the UCI Air Quality dataset to understand pollution patterns, predict concentrations of various pollutants, and provide insights for environmental monitoring and public health. By applying machine learning techniques, we aim to model the relationships between sensor responses and actual pollutant levels, addressing challenges like sensor drift and missing data. This work can contribute to better air quality management in urban areas, helping policymakers and communities make informed decisions to reduce pollution impacts.

## Partner(s)/Contributor(s)

- Karthik Mekala
- Kalyan Brata Majumder

## Methods Used

- Data Manipulation
- Data Visualization (Time-series plots, Box plots, Probability distributions, Heatmaps for correlations)
- Correlation Analysis
- Pollutant-wise Interpretation
- Machine Learning (Generalized Linear Models for CO prediction)

## Technologies

- Python

## Project Description

This project focuses on analyzing the UCI Air Quality dataset, which contains 9,358 instances of hourly averaged responses from an array of 5 metal oxide chemical sensors deployed in an Italian city from March 2004 to February 2005. The dataset includes 15 features: Date, Time, CO(GT), PT08.S1(CO), NMHC(GT), C6H6(GT), PT08.S2(NMHC), NOx(GT), PT08.S3(NOx), NO2(GT), PT08.S4(NO2), PT08.S5(O3), T (Temperature), RH (Relative Humidity), and AH (Absolute Humidity). Ground truth concentrations for pollutants like CO, NOx, NO2, and Benzene are provided by a certified analyzer.

The primary questions we are exploring include:
- How accurately can we predict pollutant concentrations using sensor data?
- What are the patterns in air quality over time and their correlations with environmental factors?
- How do we handle missing values and sensor drift in the data?

We are using data preprocessing techniques to clean the data (handling -200 missing value tags), exploratory data analysis and visualization to understand distributions and correlations, and machine learning models to predict pollutant levels. The analysis includes time-series visualizations, box plots, probability distributions, heatmaps showing correlations between pollutants and weather variables, and a correlation heatmap among pollutants with detailed pollutant-wise interpretations. A specific model is implemented to predict CO concentrations using Generalized Linear Models (GLM). Challenges include dealing with time-series nature of the data, cross-sensitivities between sensors, and concept drift affecting sensor performance.

## License

This project uses the UCI Air Quality dataset, which is licensed under a Creative Commons Attribution 4.0 International (CC BY 4.0) license. As a good practice, add LICENSE file in your project folder as well.

## Acknowledgments

We would like to express our sincere gratitude to Professor Anuj Sirohi for his invaluable guidance, insightful suggestions, clear directions, and the confidence he instilled in us to complete this project. His expertise and support were instrumental in navigating the challenges and achieving our goals.

We also thank the University of San Diego and the AAI-550 course instructors for providing the framework and resources that made this work possible.