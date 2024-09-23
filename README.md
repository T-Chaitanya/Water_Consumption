# Water Consumption of New York City (2013-2023)

## Overview

This project analyzes water consumption patterns in New York City over a ten-year period (2013-2023). Using data science techniques, we explore trends, seasonal consumption variations, borough-specific data, and perform time-series analysis to provide insights for policymakers and urban planners.

## Project Objectives

- Analyze seasonal patterns in water consumption.
- Identify water consumption percentages by borough.
- Perform time series analysis of water consumption trends.

## Data

### Description
The dataset contains water consumption details for New York City, including:
- Borough and development names.
- Revenue month, service start and end dates.
- Meter information, current charges for water and sewer, and other utility charges.

### Data Processing
1. **Data Loading**: Loaded using Python's Pandas library (`pd.read_csv()`).
2. **Data Cleaning**: 
   - Handled missing values.
   - Checked and ensured consistency in data types (e.g., numeric columns as floats/integers).
   - Identified and handled outliers based on the data's impact.

### Data Sources
- Water consumption data was sourced from relevant NYC databases and processed in CSV format.

## Methodology

### 1. Descriptive Statistics
- **Sum of Consumption**: Calculated yearly consumption (in HCF) to identify changes in seasonal consumption patterns.

### 2. Borough-Specific Consumption
- **Borough Aggregation**: Grouped data by borough to calculate total consumption for each borough, providing insights into the highest and lowest consumers.

### 3. Feature Engineering
- Converted the `Revenue Month` column to datetime format for easier analysis and extracted key date features such as year and season.
  
### 4. Time Series Analysis
- Resampled daily consumption data to yearly data to analyze consumption trends over time.

## Data Visualization

- **Seasonal Patterns**: Visualized using bar graphs to show how consumption varies across seasons and years.
- **Borough-Specific Consumption**: Created pie charts to display consumption percentages for each borough.
- **Time Series Trends**: Graphed the time series data to show the steady decline and periodic peaks in water consumption.

## Results

### 1. Seasonal Water Consumption
- Water consumption shows a general decline over the years, peaking in the summer and reaching its lowest point in the fall.
- The highest consumption occurred in 2019, while 2022 saw the lowest overall consumption.

### 2. Borough-Wise Consumption
- **Manhattan**: Highest water consumption.
- **Brooklyn**: Second-highest consumer.
- **Staten Island and Non-Development Facilities**: Lowest consumption percentages.

### 3. Time Series Trends
- **2013-2018**: A steady decline in water consumption.
- **2019**: A sudden surge, followed by a decline from 2020 to 2022.

## Tools Used

- **Python**: For data analysis and visualization.
- **Pandas**: Data loading, cleaning, and aggregation.
- **Matplotlib**: Visualization of seasonal and borough-specific consumption patterns.
  
## Conclusion

Water consumption in NYC has generally decreased from 2013 to 2023, with notable spikes and dips. Manhattan consumes the most water, while smaller boroughs such as Staten Island use significantly less. The insights from this project can help in future urban water resource planning.

## License
This project is licensed under the MIT License.

---
