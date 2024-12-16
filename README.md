# TDS_proj2

# Automated Data Analysis Report

## Overview
This repository contains a Python script for performing automated data analysis on CSV files. The script processes the provided CSV files, generates statistical summaries, identifies missing values, visualizes data distributions, and creates a narrative report on the insights derived from the dataset. 

The script uses FastAPI for API integration, OpenAI's API for generating data insights, and various data analysis libraries such as Pandas, Seaborn, and Matplotlib for visualizations.

## Files and Usage

### Input Files:
The script requires 3 CSV files as input, which will be processed to extract insights and generate visualizations. 

Example of running the script:

```bash
uv autolysis.py happiness.csv
```

## Output:
1)Summary Statistics: Basic statistics including mean, median, standard deviation, and others for each column./n
2)Missing Values: The number of missing values in each column of the dataset./n
3)Correlation Matrix: A heatmap visualizing the correlations between numerical columns./n
4)Visualizations: Three visualizations are created: Histograms of all columns, a Correlation Heatmap, and Box Plots for numerical variables./n
5)Narrative: A detailed AI-generated narrative that describes the data and insights from the analysis./n
