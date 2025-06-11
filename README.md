# Analysis-of-Global-Energy-Consumption-Renewable-Generation 🌍⚡

# Energy Consumption & Production Analysis Project 🌍⚡

## 🎓 NTI Graduation Project

This is my graduation project from the **National Telecommunication Institute (NTI)** Data Analysis Program.

### 🙏 Acknowledgments
Special thanks to **Eng. Aya Ayman** who played a crucial role in helping me reach this level of expertise, and to the **National Telecommunication Institute (NTI)** for providing this opportunity through their scholarship program.

## 📌 Project Overview

I decided to work on analyzing energy data related to consumption and production, focusing on both renewable and non-renewable energy sources. I selected a dataset from Kaggle and worked through it step-by-step to analyze and extract meaningful insights.

**Dataset Source**: [Kaggle Energy Dataset](https://www.kaggle.com/datasets/jamesvandenberg/renewable-power-generation)

## 🎯 Project Objectives

- Analyze global energy consumption and production patterns
- Compare renewable vs non-renewable energy sources
- Identify energy consumption trends by countries and continents
- Provide data-driven insights for energy policy decisions
- Create interactive visualizations for better understanding

## 🛠️ Technologies Used

### Data Analysis
- **Python** (Jupyter Notebook/Google Colab)
  - **Pandas & NumPy**: Data analysis and cleaning
  - **Matplotlib & Seaborn**: Static visualizations
  - **Plotly**: Interactive charts

### Business Intelligence
- **Power BI**
  - Power Query for data transformation
  - DAX for measures and calculations
  - Interactive dashboard creation

## 📊 Project Workflow

### Phase 1: Data Cleaning & Analysis with Python 🐍

I started by studying the data and understanding the terminology to comprehend the relationships between different columns.

#### Libraries Used:
```python
import pandas as pd
import numpy as np
import matplotlib.pyplot as plt
import seaborn as sns
import plotly.express as px

**📋 Table 1: Groups & Continents Consumption**
- Divided into Groups & Continents Consumption for better analysis
- No cleaning required
- Analyzed relationships using Pie Charts and Correlations

**📋 Table 2: Countries Consumption**
- Displays country-wise consumption data
- Changed Year data type to String to prevent calculations
- Removed duplicate entries
- Analyzed each country's consumption using Pie Charts

**📋 Table 3: Renewable Energy Sources by Year**
- Shows renewable energy sources for each year
- Changed Year data type to String (similar to Table 2)
- Analyzed the percentage of each renewable source

**📋 Table 4: Non-Renewable Energy Sources (Total)**
- Shows non-renewable energy sources as total (without yearly distribution)
- No cleaning required
- Discovered the percentage of each energy source

**📋 Table 5: Renewable Energy Production (Total)**
- Similar to Table 3 but shows renewable energy production as total
- No cleaning required
- Focused on analyzing different source percentages

**📋 Table 6: Top 20 Energy Producing Countries**
- Lists the 20 largest energy-producing countries globally
- Analyzed production capacity rankings

After Python analysis, I extracted all tables as CSV files for use in Power BI.

**Python Code**: [View in Google Colab](https://bit.ly/3tvQOwX)

### Phase 2: Data Analysis with Power BI 📊

I then moved to visual data analysis using Power BI. I faced some challenges while working on Table View but overcame them:

#### Power Query Transformations:

1️⃣ **Created Dimension Table**
   - Contains only World's Consumption & Year
   - Used for linking with other tables

2️⃣ **Created Fact Tables for:**
   - Groups Consumption
   - Continents Consumption
   - Countries Consumption
   - Renewable Power Generation
   - Used Unpivot to link tables with Dim Table (One-to-Many relationship)

3️⃣ **Merged Tables**
   - Combined Table 4 & Table 5 using Append Queries

#### Table View Enhancements:

Added new Measures and Columns to analyze consumption for each Group, Continent, and Country.

**Example**: Created Average Consumption as a Measure, then used it to create a Column that distinguishes between High and Low Consumption for Groups, Continents, and Countries.

#### Report View:

Created different pages to display results using various charts:
- **Consumption Analysis Page**: Analyzing consumption patterns
- **Generation Analysis Page**: Analyzing energy production
- **Conclusions Page**: Summary of key findings

## 🔍 Key Findings & Insights

1️⃣ **Asia is the largest energy-consuming continent globally**

2️⃣ **Tidal energy is the largest source of energy production overall**

3️⃣ **Country Energy Balance:**
   - **USA**: Consumes more energy than it produces
   - **Ukraine**: Produces more than it consumes, providing opportunities for energy export and increased revenue

4️⃣ **High Consumption Statistics:**
   - 76.71% of Groups are classified as High Consumption
   - 69.91% of Countries are classified as High Consumption

## 📈 Visualizations

### Python Visualizations
- Pie charts for consumption distribution
- Correlation matrices for relationships
- Interactive plots using Plotly

### Power BI Dashboard Features
- Interactive filters by year, country, and energy type
- Drill-down capabilities for detailed analysis
- Dynamic measures for real-time calculations

## 🚀 How to Use This Project

### Running the Python Analysis:

1. **Option 1 - Google Colab (Recommended)**:
   - Open the [Colab Notebook](https://bit.ly/3tvQOwX)
   - Run all cells sequentially

2. **Option 2 - Local Environment**:
   ```bash
   # Clone the repository
   git clone https://github.com/yourusername/energy-analysis.git
   
   # Install required libraries
   pip install pandas numpy matplotlib seaborn plotly
   
   # Run the notebook
   jupyter notebook energy_analysis.ipynb
