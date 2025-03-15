# Carbon Emissions Impact Analysis

## Overview
In this analysis, I explore the impact of carbon emissions on global temperatures. The focus is on identifying historical trends, detecting anomalies, and simulating potential future scenarios to understand how changes in CO₂ concentrations influence temperature anomalies.

## Datasets Used
I use two primary datasets:
1. **Temperature Data**: Annual temperature anomalies measured in degrees Celsius across decades.
2. **CO₂ Data**: Monthly global atmospheric CO₂ concentrations in parts per million (ppm).

By combining these [datasets](https://statso.io/carbon-emissions-worldwide-case-study/), I investigate correlations, detect patterns over decades, and use predictive modeling to simulate "what-if" scenarios. This data-driven approach provides actionable insights into the connection between carbon emissions and climate change, offering valuable context for sustainable policy-making.

---

## Carbon Emissions Impact Analysis with Python

### Importing Required Libraries and Loading Datasets
I start by importing necessary Python libraries and loading the dataset.

### Key Statistics Calculation
I calculate key statistics for temperature changes and CO₂ concentrations:
- **Mean Temperature Change**: 0.54°C
- **Median Temperature Change**: 0.47°C
- **Variance of Temperature Anomalies**: 0.43
- **Mean CO₂ Concentration**: 180.72 ppm
- **Median CO₂ Concentration**: 313.84 ppm
- **Variance of CO₂ Concentrations**: 32,600

This analysis highlights the stronger fluctuation in CO₂ data compared to temperature changes.

---

## Time-Series Analysis
Examining how temperature changes and CO₂ concentrations evolve over time:
- A consistent increase in CO₂ concentrations suggests greenhouse gas accumulation.
- A slight upward trend in global temperature change supports the hypothesis of CO₂’s contribution to global warming.

![Time-Series Graph](https://github.com/Sourabh1710/Analysis-of-Impact-of-Carbon-Emissions/blob/main/images/Time-Series%20of%20Temperature%20Change%20and%20CO2%20Concentration.png)

A **heatmap** reveals a strong positive correlation (0.96) between CO₂ concentrations and temperature changes, reinforcing the connection between emissions and warming trends.

![Heatmap](https://github.com/Sourabh1710/Analysis-of-Impact-of-Carbon-Emissions/blob/main/images/Correlation%20Heatmap.png)

A **scatter plot** displays a linear trend where higher CO₂ concentrations correspond to greater temperature changes.

![Scatter Plot](https://github.com/Sourabh1710/Analysis-of-Impact-of-Carbon-Emissions/blob/main/images/Temperature%20Change%20vs%20CO2%20concentrations.png)

---

## Trends and Seasonal Variations Analysis
Using linear regression:
- **CO₂ trend slope**: 0.32 (indicating rapid increase)
- **Temperature trend slope**: 0.03 (indicating steady accumulation over time)

![Linear Regression Trends](https://github.com/Sourabh1710/Analysis-of-Impact-of-Carbon-Emissions/blob/main/images/Trends%20in%20Temperature%20Change%20and%20CO2%20concentrations.png)

**Seasonal fluctuations in CO₂ concentrations**:
- Peak in late spring/early summer (around May)
- Lowest in fall (around September)

This seasonal cycle underscores the role of natural carbon sinks in moderating atmospheric CO₂ levels.

![Seasonal Variations Graph](https://github.com/Sourabh1710/Analysis-of-Impact-of-Carbon-Emissions/blob/main/images/Seasonal%20Variations%20in%20CO2%20Concentrations.png)

---

## Correlation and Causality Analysis
To quantify the relationship between CO₂ and temperature anomalies, I compute:
- **Pearson Correlation**: 0.9554 (strong linear relationship)
- **Spearman Correlation**: 0.9379 (strong monotonic relationship)

### Granger Causality Test Results:
| Lag | p-value | Significance |
|-----|---------|-------------|
| 1   | 0.0617  | Weak evidence for causality |
| 2   | 0.6754  | No evidence |
| 3   | 0.2994  | No evidence |

While correlation is strong, the Granger Causality test does not confirm direct causality within the tested lags.

---

## Lagged Effects Analysis
I analyze whether CO₂ concentrations from previous years influence current temperature anomalies by using an **Ordinary Least Squares (OLS) regression model**:
- **R-squared value**: 0.949 (94.9% variance explained)
- **CO₂ coefficient**: 0.3245 (statistically significant, p < 0.05)

---

## Clustering Climate Patterns
I group years based on similarities in temperature anomalies and CO₂ concentrations using **K-Means clustering**:
- **Clusters**:
  - Low CO₂ and temperature (Green)
  - Moderate CO₂ and temperature (Orange)
  - High CO₂ and temperature (Blue)

The transition from green to blue clusters reflects increasing temperature change corresponding to rising CO₂ levels.

![Clustering Graph](https://github.com/Sourabh1710/Analysis-of-Impact-of-Carbon-Emissions/blob/main/images/Clustering%20of%20Years%20Based%20on%20Climate%20Patterns.png)

---

## Predicting Temperature Changes Under "What-If" Analysis
Using a **simple linear regression model**, I simulate temperature impacts under different emission scenarios:

| Scenario | Predicted Temperature Change |
|----------|------------------------------|
| CO₂ +10% | Notable rise in temperature anomalies |
| CO₂ -10% | Significant cooling effect |
| CO₂ +20% | Greater impact on warming |
| CO₂ -20% | Potential reversal of warming trends |

These findings emphasize the sensitivity of global temperatures to CO₂ levels, highlighting the importance of emissions reduction.

---

## Summary
My analysis highlights:
- A **strong correlation** between CO₂ concentrations and global temperature anomalies.
- **Time-series and clustering analyses** revealing trends of escalating emissions driving temperature increases.
- **Seasonal variations** emphasizing natural carbon sinks' role.
- **Lagged effects analysis** indicating current CO₂ levels have the strongest impact on temperature changes.
- **Predictive modeling** showing even modest emission reductions can significantly mitigate global warming.

These findings underline the urgent need for actionable policies to address climate change effectively.

---
## Author

Sourabh Sonker <br>
Data Scientist

