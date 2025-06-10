# Advertising Sales Prediction Model

![Python](https://img.shields.io/badge/Python-3.8%2B-blue)
![Scikit-learn](https://img.shields.io/badge/Scikit--learn-1.0%2B-orange)
![Pandas](https://img.shields.io/badge/Pandas-1.3%2B-brightgreen)
![Matplotlib](https://img.shields.io/badge/Matplotlib-3.5%2B-blueviolet)

A machine learning project that analyzes the impact of different advertising channels (TV, Radio, Newspaper) on product sales using Linear Regression.

## Table of Contents
- [Project Overview](#project-overview)
- [Dataset](#dataset)
- [Features](#features)
- [Exploratory Data Analysis](#exploratory-data-analysis)
- [Modeling Approach](#modeling-approach)
- [Results](#results)
- [Key Insights](#key-insights)
- [Installation](#installation)
- [Usage](#usage)
- [Future Improvements](#future-improvements)

## Project Overview
This project builds a predictive model to analyze the impact of different advertising budgets (TV, Radio, Newspaper) on product sales. The goal is to understand which advertising channel contributes most to revenue and help businesses optimize their marketing spend.

## Dataset
The dataset contains 200 records of advertising budgets and corresponding sales figures. Original data source: [Advertising Dataset](https://www.kaggle.com/datasets).

## Features
- **TV Ad Budget ($)** - Amount spent on TV advertisements
- **Radio Ad Budget ($)** - Amount spent on radio advertisements
- **Newspaper Ad Budget ($)** - Amount spent on newspaper ads
- **Sales ($)** (Target Variable) - Revenue generated

## Exploratory Data Analysis
Key findings from EDA:
- No missing values in the dataset
- TV and Radio ads showed higher correlation with sales than newspaper ads
- Sales distribution was approximately normal
- Clear trend in sales over time

![Correlation Heatmap](images/correlation_heatmap.png)
*Feature correlation heatmap showing relationships between variables*

## Modeling Approach
- Used **Linear Regression** for interpretable coefficients
- Split data into 80% training and 20% testing sets
- Scaled features using StandardScaler
- Evaluated using MAE, MSE, and R² metrics

## Results
**Training Set Performance:**
- MAE: 1.20
- MSE: 2.71
- R²: 0.90

**Testing Set Performance:**
- MAE: 1.46
- MSE: 3.17
- R²: 0.90

The model explains 90% of the variability in sales (R² = 0.90), demonstrating strong predictive power.

## Key Insights
1. **TV Ads** contributed most significantly to sales (highest coefficient)
2. **Radio Ads** also had strong impact, though slightly less than TV
3. **Newspaper Ads** showed minimal effect on sales

**Business Impact:** Marketing teams can use these insights to:
- Allocate more budget to high-impact channels (TV and Radio)
- Reduce spending on less effective channels (Newspaper)
- Optimize overall marketing ROI

## Installation
1. Clone this repository:
   ```bash
   git clone https://github.com/yourusername/advertising-sales-prediction.git
   cd advertising-sales-prediction
