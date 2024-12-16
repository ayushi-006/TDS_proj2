# TDS_proj2

# Automated Data Analysis Report

## Overview

This repository provides a robust **Automated Data Analysis Tool** that enables users to perform comprehensive exploratory data analysis (EDA) on any dataset with minimal effort. The tool computes summary statistics, identifies missing values, detects outliers, and generates insightful visualizations to better understand the data.

The script uses FastAPI for API integration, OpenAI's API for generating data insights, and various data analysis libraries such as Pandas, Seaborn, and Matplotlib for visualizations.

## Files and Usage

### Input Files:
The script requires 3 CSV files as input, which will be processed to extract insights and generate visualizations. 

# Automated Data Analysis Tool
## Features

- **Data Insights**: Summary statistics and correlation matrices for numerical data.
- **Outlier Detection**: Identifies anomalies using the Interquartile Range (IQR) method.
- **Visualizations**: Auto-generates plots such as:
  - Correlation Heatmap
  - Outlier Distribution
  - Numerical Data Distribution
- **Detailed Reporting**: Creates a `README.md` file summarizing the analysis and insights.

## Prerequisites

- Python 3.9 or higher
- Required Python libraries:
  - `pandas`
  - `numpy`
  - `matplotlib`
  - `seaborn`
  - `scikit-learn`
  - `openai`

## Usage

### Command-Line Execution

Run the script with the following command:

```bash
uv autolysis.py <path_to_csv_file>
```

This command will:
- Analyze the dataset
- Generate summary statistics
- Detect outliers
- Create visualizations
- Produce a detailed `README.md` file with results

### Outputs

All outputs, including visualizations and the `README.md` report, will be saved in the current directory.

## Example Outputs

### Summary Statistics

The tool provides descriptive statistics for all numerical columns:

| Statistic    | Column1 | Column2 | ... |
|--------------|---------|---------|-----|
| Mean         | 12.34   | 56.78   | ... |
| Std Dev      | 1.23    | 4.56    | ... |
| Min          | 10.00   | 50.00   | ... |
| 25th Percentile | 11.00 | 52.00 | ... |
| Median       | 12.00   | 55.00   | ... |
| 75th Percentile | 13.00 | 58.00 | ... |
| Max          | 14.00   | 60.00   | ... |

### Missing Values

A summary of missing data:

| Column       | Missing Values Count |
|--------------|-----------------------|
| Column1      | 3                     |
| Column2      | 0                     |

### Visualizations

#### Correlation Heatmap

This heatmap shows the relationships between numerical variables:

![image](https://github.com/user-attachments/assets/f6c19e22-ac80-40c7-8429-2758735ebb3c)

#### Outliers Detection

Bar chart indicating the number of outliers in each column:

![image](https://github.com/user-attachments/assets/42f930d3-626e-487f-a059-b4e126a35d6d)

#### Distribution of Data

Distribution plot for the first numerical column:

![image](https://github.com/user-attachments/assets/16810839-6737-46ca-a678-5eccacb8bb52)

## LLM-Generated Story

This tool leverages an AI-powered language model to create a data-driven story based on the analysis. The story provides insights and highlights significant trends and patterns in the dataset.

## Contribution
welcome contributions! Feel free to submit issues or pull requests to improve the functionality or documentation.

## License

This project is licensed under the MIT License. See the LICENSE file for details.

---
