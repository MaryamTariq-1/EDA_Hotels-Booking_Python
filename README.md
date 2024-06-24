# EDA_Hotels-Booking_Python

## Table of Contents

- [Overview](#overview)
- [Dataset](#dataset)
- [Data Cleaning](#data-cleaning)
- [Exploratory Data Analysis](#exploratory-data-analysis)
  - [Univariate Analysis](#univariate-analysis)
  - [Bivariate Analysis](#bivariate-analysis)
  - [Multivariate Analysis](#multivariate-analysis)
- [Key Insights](#key-insights)
- [How to Run](#how-to-run)
- [Conclusion](#conclusion)
- [Acknowledgements](#acknowledgements)

## Overview

This project is part of my internship at CodexCue, where I performed an in-depth analysis of a hotel booking dataset containing 119,390 entries. The goal was to clean the data, conduct exploratory data analysis (EDA), and uncover meaningful insights about booking trends, customer behaviors, and other key metrics.

## Dataset

The dataset used in this analysis contains various features related to hotel bookings, including:

- Hotel type
- Booking lead time
- Arrival date
- Number of weekend and weeknight stays
- Number of adults, children, and babies
- Meal type
- Country of origin
- Market segment
- Distribution channel
- Booking status (canceled or not)
- Room type reserved and assigned
- Special requests and more

## Data Cleaning

### Steps Taken:

1. **Identified and Filled Missing Values**:
    - `children`: Filled with the median value.
    - `country`: Filled with the mode value.
    - `agent` and `company`: Filled with `0` to indicate 'no agent' and 'no company'.

2. **Data Type Conversion**:
    - Converted `reservation_status_date` to datetime format.

## Exploratory Data Analysis

### Univariate Analysis
- Analyzed the distribution of individual variables using histograms and summary statistics.

### Bivariate Analysis
- Examined relationships between pairs of variables:
  - **Lead Time vs ADR (Average Daily Rate)**: Scatter plot and correlation analysis.
  - **ADR vs Hotel Type**: Box plot and violin plot.
  - **Hotel Type vs Cancellation Status**: Contingency table and heatmap.

### Multivariate Analysis
- Utilized advanced visualization techniques:
  - **Pair Plot**: For multiple numerical variables.
  - **Correlation Heatmap**: For numerical variables.
  - **Facet Grid**: For ADR by hotel type conditioned on cancellation status.
  - **3D Scatter Plot**: For lead time, ADR, and stays in week nights.
  - **Parallel Coordinates Plot**: For multi-dimensional data visualization.

## Key Insights

- **Lead Time and ADR**: Found patterns in booking lead times and their correlation with pricing.
- **Hotel Type and Cancellation**: Analyzed how hotel type impacts cancellation rates.
- **Customer Segments**: Identified different customer segments based on booking behaviors and special requests.

## How to Run

1. Clone the repository:
    ```sh
    git clone https://github.com/MaryamTariq-1/hotel-booking-analysis.git
    ```

2. Run the analysis script:
    ```sh
    jupyter notebook hotel_booking_analysis.ipynb
    ```

## Conclusion

This analysis provided valuable insights into hotel booking patterns and customer behaviors. The results can help in making data-driven decisions for improving customer satisfaction and optimizing hotel operations.

## Acknowledgements

I would like to thank CodexCue for providing this opportunity and supporting me throughout this project.

