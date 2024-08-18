# L6 Data Science Professional Practice 
Year 1 Term 3 
Hate-Crime

## FBI Hate Crime

![Image URL](https://cdn.statcdn.com/Infographic/images/teaser/16100.jpeg)

## Research Question
How have significant periods of social unrest between 1991 and 2022 impacted reported hate crime rates in the United States, and what are the projected trends for 2030?

## Executive Summary
This project examines the connection between periods of social unrest and reported hate crimes in the USA over a 30-year period. Understanding this relationship is vital for policymakers, law enforcement, and community leaders who seek to address and reduce these detrimental acts.

## Methods

### Data Collection

### Source
Reported Hate Crime data from 1991 to 2022, sourced from FBI public data sets (FBI Hate Crime Data Set), alongside data on periods of social unrest in the United States during the same timeframe, primarily gathered from Wikipedia (Wikipedia Social Unrest Data Source).

### Variables
Key variables in the hate crime data include the incident data, offense type, location, and bias description. Essential variables in the social unrest data include the data, bias description, and location.

### Data Preparation / Cleaning

#### Hate Crime Data Set
Offence names were categorised into first, second, and third level groups based on the primary offence. Likewise, location names were grouped into first and second level categories according to the primary location. Bias descriptions were also organised into first, second, and third level groups based on the primary bias description.

#### Social Unrest Data Set
The data, initially presented in a single column, was split to include year, month (if applicable), type of unrest, location, and bias targeted. Locations were aggregated into first and second level categories, while the bias categories were organised into first, second, and third level groups.

## Data Analytics

### Techniques Used
The statistical method I plan to use combines Interrupted Time Series Analysis with either ARIMA or Negative Binomial Regression models.

### Justification of Methods
Interrupted Time Series Analysis enables the examination of changes in the level and trend of hate crimes before and after the unrest periods. Negative Binomial Regression enables the analysis of count data with overdispersion for studying the relationship between social unrest and hate crime incidences over a long period. AutoRegressive Integrated Moving Average (ARIMA) is used for analysing and forecasting time series data and is particularly useful for data that show patterns over time.

## Results

### Data Communication Tools

#### Screenshots and Narrative

## Discussion / Recommendations

## References
- [FBI Hate Crime Data Set](https://cde.ucr.cjis.gov/LATEST/webapp/#/pages/downloads#datasets)
- [Wikiepedia Social Unrest Data Source](https://en.wikipedia.org/wiki/List_of_incidents_of_civil_unrest_in_the_United_States#1990%E2%80%931999)
