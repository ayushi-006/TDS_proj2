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

1. **Summary Statistics**: Basic statistics including mean, median, standard deviation, and others for each column.
2. **Missing Values**: The number of missing values in each column of the dataset.
3. **Correlation Matrix**: A heatmap visualizing the correlations between numerical columns.
4. **Visualizations**: Three visualizations are created: Histograms of all columns, a Correlation Heatmap, and Box Plots for numerical variables.
5. **Narrative**: A detailed AI-generated narrative that describes the data and insights from the analysis.


## How it Works

1. **Data Import**: The script begins by loading the input CSV files into a Pandas DataFrame.
2. **Data Analysis**: It performs an analysis to compute summary statistics, detect missing values, and generate a correlation matrix.
3. **Data Visualizations**:
   - **Histograms** are generated for each column to display the distribution of values.
   - **Correlation Heatmap** is generated to visually represent correlations between numerical variables.
   - **Box Plots** are produced for numerical columns to show their distributions and detect any outliers.
4. **Narrative Generation**: The script sends the analysis results (summary statistics, missing values, and correlation matrix) to OpenAI’s API to generate a narrative that provides insights into the data.
5. **Markdown Report**: The final results are written to a `README.md` file, including the statistical summaries, missing value counts, correlation matrix, generated narrative, and visualizations.

## Data Insights

### Summary Statistics
- **Columns**: Each dataset's columns are listed to provide a quick reference.
- **Summary Statistics**: Key statistical metrics like mean, standard deviation, min, max, and percentiles for each column in the dataset.

### Missing Values
- A detailed count of missing values for each column, allowing for the identification of columns that require cleaning or imputation.

### Correlation Matrix
- A heatmap showing the correlation between numerical columns. This can be used to understand relationships between variables.

### AI-Generated Narrative
The AI model generates insights by analyzing the patterns and relationships in the data. Some potential insights include:
- Which variables are strongly correlated.
- Whether any variables exhibit high variance or potential outliers.
- Key trends observed in the data, such as any significant skew or anomalies in distributions.

## Visualizations
The following visualizations are included in the report:
1. **Histograms**: Distribution of values across all columns.
2. **Correlation Heatmap**: Visual representation of correlations between numerical variables.
3. **Box Plots**: Distributions of numerical variables, highlighting outliers.
