Electricity Demand Forecasting

Overview

This repository contains a mini research project on electricity demand forecasting using historical hourly electricity demand data. The study investigates the ability of machine learning and time-series forecasting methods to model electricity demand and generate future forecasts.

Two forecasting approaches are evaluated:
HistGradientBoosting
SARIMAX

The project includes data analysis, model development, forecasting, evaluation, visualization, and residual analysis.

Research Objective
The main objective of this study is to investigate and compare forecasting approaches for predicting future electricity demand using historical hourly observations.

The project focuses particularly on the performance of the HistGradientBoosting model for predicting future electricity demand, while SARIMAX is used as a time-series forecasting approach for comparison.

Dataset
The analysis uses the PJME hourly electricity demand dataset.

The dataset contains historical hourly electricity demand observations and is stored in:
Data/PJME_hourly.csv

Methodology

The research workflow consists of the following stages:

Data loading and preparation

Exploratory data analysis

Data preprocessing

Feature preparation

Model development

Forecast generation

Model evaluation

Residual analysis

Comparison and discussion of results

Models

HistGradientBoosting

HistGradientBoosting is a gradient-boosting machine learning algorithm used to model nonlinear relationships between predictors and electricity demand.

The model was evaluated using forecasting metrics and visual comparisons between actual and predicted electricity demand.

SARIMAX

SARIMAX is a statistical time-series model that incorporates autoregressive, differencing, moving-average, and seasonal components.

It was implemented as a comparative forecasting approach.

Model Evaluation

The models were evaluated using forecasting performance metrics and graphical analysis.

The evaluation includes:

Actual versus forecast values

Forecast performance metrics

Forecast plots

Residual distribution

Residual analysis

Autocorrelation analysis

Results

The project examines how effectively the models reproduce observed electricity demand and their ability to generate forecasts of future demand.

Particular attention is given to the performance of the HistGradientBoosting model in predicting future electricity demand.

The detailed results, figures, discussion, strengths, weaknesses, and conclusions are provided in the research report.

Residual Analysis

Residual diagnostics were conducted to assess the behavior of the forecasting errors.

The analysis includes examination of the residual distribution and autocorrelation. The residual analysis provides additional information about model adequacy and remaining patterns in the forecasting errors.

Repository Structure

electricity-demand-forecasting/
│
├── Code/
│   ├── sarimax_forecasting.ipynb
│   └── HistGradientBoosting_forecasting.ipynb
│
├── Data/
│   └── PJME_hourly.csv
│
├── Report/
│   ├── research report.doc
│   └── electricity-demand-forecasting-report.pdf
│
└── README.md

How to Run

Clone or download the repository and open either notebook using Jupyter Notebook or JupyterLab.

The notebooks load the dataset using a relative path:

PJ = pd.read_csv("../Data/PJME_hourly.csv")

This allows the code to work within the repository structure without relying on a personal Windows file path.

Requirements

The project uses Python and common data science and forecasting libraries, including:

pandas
NumPy
scikit-learn
statsmodels
Matplotlib
Jupyter Notebook

Research Report

The complete research report is available in the Report folder.

Conclusion
This project demonstrates the application of both machine learning and statistical time-series methods to electricity demand forecasting. It provides a reproducible workflow covering data preparation, model development, forecasting, evaluation, and diagnostic analysis.
