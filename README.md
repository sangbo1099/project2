# Project 2

## Project Overview

This project processes and visualizes air quality data from Raleigh-Durham Airport to explore patterns in three major pollutants: Carbon Monoxide (CO), Particulate Matter 2.5 (PM2.5), and Ozone (O3). The analysis includes:

-   **Custom Data Processing Function**: Developed a reusable function to clean and standardize messy EPA air quality measurements
-   **Multi-Year Data Integration**: Applied the processing function across three years of data (2018-2020)
-   **Exploratory Visualizations**: Created two plots examining temporal patterns:
    -   Monthly averages of CO and O3 concentrations across all years with 95% confidence intervals
    -   Monthly PM2.5 concentrations with year-by-year comparisons

## Project Structure

```         
project2/
│
├── README.md                  # This file
├── Yoon_Sang_Bo_Project2.Rmd  # Main analysis R Markdown file
├── Yoon_Sang_Bo_Project2.docx # Knitted Word output
│
└── data/                      # Raw data files
    ├── AQ_2018.csv
    ├── AQ_2019.csv
    └── AQ_2020.csv
```

## Methods

### Data Processing

A custom function was developed to clean and process the raw air quality data:

1.  **Variable Renaming**: Simplified pollutant column names for easier manipulation
2.  **Date Formatting**: Converted date character strings to proper date objects
3.  **Daily Averaging**: Calculated mean concentrations for days with multiple pollutant measurements
4.  **Duplicate Removal**: Eliminated duplicate rows
5.  **Error Correction**: Set negative concentration values (measurement errors) to zero

This function was then applied to all 3 datasets in preparation for further exploratory data analysis.

### Visualization

Two primary visualizations were created:

1.  **CO and O3 Monthly Trends**: Displays average monthly concentrations across all years with 95% confidence intervals
2.  **PM2.5 Temporal Patterns**: Shows PM2.5 concentrations by month, separated by year

## Author

Sang Bo Yoon\
<https://github.com/sangbo1099/project2>
