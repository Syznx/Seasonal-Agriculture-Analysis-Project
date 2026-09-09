# 🌾 Seasonal Agricultural Performance Analysis Project

## Overview
This project, **"Seasonal Agricultural Performance Analysis"**, delves into a dataset containing information on 4,000 farms across various seasons (Kharif, Rabi, Zaid) and 28 features. The primary objective is to analyze how agricultural performance varies across these seasons and to identify meaningful patterns concerning environmental conditions, resource usage, production, and economic outcomes.

## Dataset
- **Name**: Seasonal Agriculture Performance Dataset
- **Records**: 4,000 farms
- **Features**: 28 environmental, resource, production, and economic variables.
- **Seasons Covered**: Kharif, Rabi, Zaid

## Technical Stack
- **Language**: Python
- **Libraries**: 
  - `pandas`: For data manipulation and analysis.
  - `numpy`: For numerical operations.
  - `matplotlib`: For creating static, interactive, and animated visualizations.
  - `seaborn`: For high-level statistical data visualization.

## Project Structure & Analysis Sections

### 1. Data Loading and Preprocessing
- Initial loading of the dataset.
- Handling missing values through imputation (median for `Rainfall_mm`, `Soil_Moisture_pct`, and season-wise median for `Yield_Tonnes_Ha`).

### 2. Environmental Conditions Across Seasons
- **Analysis**: Visualizing the distribution of `Rainfall_mm`, `Avg_Temperature_C`, and `Humidity_pct` across Kharif, Rabi, and Zaid seasons using box plots.
- **Key Finding**: Kharif is the most environmentally intense season (highest rainfall, humidity, and weather variation), while Zaid is consistently hot and dry.

### 3. Economic Analysis Across Seasons
- **Analysis**: 
  - Correlation heatmap of key economic and environmental features.
  - Bar plots comparing `Total_Cost_INR`, `Revenue_INR`, and `Profit_INR` by season.
  - Box plot showing `Profit_INR` distribution per season.
- **Key Findings**: 
  - Kharif is the most profitable season.
  - Zaid is the most financially risk-prone season, often incurring losses.
  - Most farms operate near break-even, with significant profits confined to large-scale outliers.

### 4. Resource Usage Across Seasons
- **Analysis**: 
  - Box plots for `Water_Used_m3` and `Fertilizer_kg_ha` by season.
  - Bar chart showing irrigation method frequency.
  - Water efficiency comparison across irrigation methods.
- **Key Findings**: 
  - Water usage is highest in Zaid, contributing to its poor profitability.
  - Flood irrigation is the most popular but least efficient method (3.44 t/1000m3).
  - Rainfed farming is the most efficient (7.56 t/1000m3), but rainfall dependency is a risk.

### 5. Production Analysis
- **Analysis**: 
  - Bar charts for total production by season and top 10 crops by production.
  - Identification of top-producing states and best crops per season.
- **Key Findings**: 
  - Kharif is the most productive season overall.
  - Sugarcane dominates production across all seasons.
  - Punjab is the highest-producing state.
  - Zaid's low production further explains its poor profitability.
  - High production volume alone does not guarantee profitability.

### 6. Disease & Pest Risk Analysis
- **Analysis**: 
  - Box plot showing `Disease_Pest_Risk_pct` by season.
  - Scatter plot of `Disease_Pest_Risk_pct` vs `Yield_Tonnes_Ha`.
  - Correlation calculation between disease risk and yield.
- **Key Findings**: 
  - Kharif has the highest disease and pest risk due to high humidity and rainfall.
  - The correlation between disease risk and yield is negligible (0.014), suggesting effective management or stronger influence from other factors.

## Overall Conclusion
Analysis revealed clear seasonal patterns. While Kharif is the most productive and profitable, most farmers across all seasons struggle to achieve significant profits. The high costs associated with resource usage (especially water in Zaid) and potential inefficiencies in traditional farming methods significantly impact profitability.

## Recommendations
1.  **Promote Drip Irrigation**: Especially in the Zaid season, to reduce water waste and costs.
2.  **Shift Focus from Zaid Farming**: Encourage reallocation of resources to more viable seasons (Kharif) for small farmers due to high costs and low profitability.
3.  **Crop Diversification**: Reduce over-reliance on single crops like Sugarcane to mitigate market risks and stabilize farmer income.

## How to Run the Project
1.  **Environment**: This notebook is designed to run in Google Colab.
2.  **Dataset**: Ensure the `seasonal_agriculture_performance_dataset (3).csv` file is uploaded to your Colab environment or the specified path (`/content/seasonal_agriculture_performance_dataset (3).csv`).
3.  **Execution**: Run all cells sequentially in the notebook.

## Author
- **Harshit Saini**
- **Institution**: Engineering College Ajmer, Rajasthan

