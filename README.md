# L6 Data Science Professional Practice 
Year 1 Term 3 
Hate-Crime

## FBI Hate Crime

![Image URL](https://cdn.statcdn.com/Infographic/images/teaser/16100.jpeg)

## Research Question
How have significant periods of social unrest between 1991 and 2022 impacted reported hate crime rates in the United States, and what are the projected trends for 2030?

## Executive Summary
This project investigates the relationship between periods of social unrest and reported hate crimes in the USA over the past 30 years. By analysing historical data on both social disturbances and hate crime incidents, the project seeks to uncover how significant events such as protests, riots, and civil unrest influence the frequency and nature of hate crimes. Understanding this relationship is essential for policymakers, law enforcement, and community leaders, as it provides insights into how social tensions can exacerbate hate-driven behaviour. With this knowledge, stakeholders can develop more effective, targeted strategies to prevent and address hate crimes. The ultimate goal is to foster safer, more inclusive communities by addressing the underlying factors that contribute to these incidents and improving response mechanisms during times of social unrest.

## Introduction / Project Background

Identifying how different variables impact hate crime is essential for several key reasons. Firstly, it helps to uncover the underlying causes and contributing factors that lead to the perpetration of hate crimes (Analysis of hate crimes, 2024). By understanding these influences—whether they be social, economic, political, or cultural—authorities and communities can better predict when and where such crimes are likely to occur, allowing for more effective prevention measures.
Secondly, recognising the variables that drive hate crime provides a foundation for developing targeted interventions. For example, if economic hardship or political rhetoric is found to be a significant factor, strategies can be designed to address these specific issues, potentially reducing the likelihood of hate crimes occurring.

Furthermore, understanding the impact of various variables on hate crime is crucial for shaping policies and educational programmes aimed at reducing prejudice and promoting tolerance. This insight enables policymakers, educators, and community leaders to address the root causes of hate, rather than just its symptoms, fostering long-term societal change.
Ultimately, identifying these variables not only aids in reducing the incidence of hate crime but also contributes to creating a more just and inclusive society, where all individuals feel safe and valued.

## Methods

### Data Collection

### Source
This project uses reported Hate Crime data from 1991 to 2022, which has been sourced from FBI public data sets (FBI 2023). To complement this, data on periods of social unrest in the United States within the same timeframe has been collected, primarily gathered from Wikipedia (Wikipedia 2024).

### Variables
Key variables in the hate crime data include the data of the incident, the type of offense committed, the geographic location of the crime, and a description of the bias or motivation behind the act.

In the social unrest data, essential variables include the date of the unrest, a description of the underlying issues or biases driving the unrest, and the geographic location where the events occurred.

### Data Preparation / Cleaning

For the hate crime data, offence names and bias descriptions were categorised into first, second, and third level groups based on their primary characteristics, while locations were grouped into first and second level categories. Social unrest data, initially in a single column, was separated into year, month, type of unrest, location, and bias, with locations and biases similarly categorised. Additional cleaning and research were needed due to the public nature of the data.

## Data Analytics

### Techniques Used
To examine the connection between periods of social unrest and reported hate crime, I plan to use a combination of Interrupted Time Series Analysis (ITSA) and either an ARIMA model or a Negative Binomial Regression model. ITSA will allow us to assess changes in hate crime trends before, during, and after periods of unrest. The ARIMA model will help analyse time series data with trends and seasonal patterns, while the Negative Binomial Regression model is suited for over dispersed count data. Together, these techniques will provide a detailed understanding of how social unrest impacts hate crime rates.

### Justification of Methods
Interrupted Time Series Analysis allows for the examination of changes in both the level and trend of hate crimes before, during, and after periods of social unrest. This method helps identify whether significant shifts occur as a result of these events. Negative Binomial Regression is used to analyse count data, particularly when overdispersion is present, making it ideal for studying the relationship between social unrest and hate crime incidences over an extended period. The AutoRegressive Integrated Moving Average (ARIMA) model is employed for analysing and forecasting time series data, especially when the data exhibit trends or patterns over time. This combination of methods ensures a comprehensive analysis of how social unrest impacts hate crime rates across different timeframes.

## Results

### Data Communication Tools

#### Screenshots and Narrative

## Recommendations

Projecting the impact of social unrest on reported hate crimes is challenging due to several key limitations. Inconsistent data, underreporting (the hate crime reporting, 2017), and varying regional practices complicate accuracy. Establishing a direct link between unrest and hate crimes is difficult because other factors, such as economic stress or media influence, may also play a role. Timing discrepancies, regional differences, media distortion, and government actions further complicate projections. 

Additionally, the varying short- and long-term effects of social unrest require careful modelling. Collecting and integrating inconsistent data from multiple sources adds to these challenges, as variations in data quality and reporting practices, along with gaps due to underreporting, reduce reliability. These factors necessitate a cautious and nuanced approach to data analysis, accounting for uncertainties and contextual nuances.

## Discussion and Conclusion

## References
1.	FBI Hate Crime Data Set, 2023, [online] Available CDE(cjis.gov) [Accessed 2024]
2.	Wikipedia List of Civil Unrest, 2024, [online] Available: List of incidents of civil unrest in the United States - Wikipedia [Accessed 2024]
3.	The hate crime reporting gap & why it matters, 2017, [online] Available: The Hate Crimes Reporting Gap & Why It Matters | Not in Our Town (niot.org) [Accessed 2024]
4.	Analysis of Hate Crimes in the United States, 2024, [online] Available: Analysis of Hate Crime Rates in the United States: Statistical Modeling of Public Safety Issues Based on Socioeconomic Factors | IEEE Conference Publication | IEEE Xplore [Accessed 2024]
5.	U.S. Hate Crime Investigation Rates and Characteristics, 2021, [online] Available: U.S. Hate Crime Investigation Rates and Characteristics: Findings from the National Hate Crime Investigations Study (NHCIS) (ojp.gov) [Accessed 2024]
6.	Learn About Hate Crimes, 2024, [online] Available: Hate Crimes | United States Department of Justice | Hate Crimes | Learn More [Accessed 2024]
7.	Crime type definitions, 2024, [online] Available: Crime type definitions | Metropolitan Police [Accessed 2024]
8.	Designing Buildings, 2024, [online] Available: Purpose group - Designing Buildings [Accessed 2024]
9.	
10.	
11.	
12.	
13.	
14.	
15.	
