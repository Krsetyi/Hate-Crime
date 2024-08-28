# L6 Data Science Professional Practice 
Year 1 Term 3 
Hate-Crime

## FBI Hate Crime

![Image URL](https://cdn.statcdn.com/Infographic/images/teaser/16100.jpeg)

## Research Question
How have significant periods of social unrest between 1991 and 2022 impacted reported hate crime rates in the United States, and what are the projected trends for 2030?

## Executive Summary
This project explores the relationship between periods of social unrest and reported hate crimes in the USA over the past 30 years. By analysing historical data on social disturbances and hate crime incidents, the research seeks to uncover how significant events—such as protests, riots, and civil unrest—influence the frequency and nature of hate crimes.

Understanding this connection is essential for policymakers, law enforcement, and community leaders. The insights gained can help these stakeholders recognise how social tensions may exacerbate hate-driven behaviour, enabling them to develop more effective, targeted strategies for preventing and addressing hate crimes. The overarching aim is to promote safer, more inclusive communities by addressing the root causes of these incidents and enhancing response strategies during times of social unrest.

The findings from the ITSA model indicate that factors not included in the analysis may impact the reporting of hate crimes. Since a direct correlation between periods of social unrest and hate crimes in the United States from 1991 to 2022 could not be established, making a reliable prediction for 2030 remains unfeasible.


## Introduction / Project Background

Identifying how different variables impact hate crime is essential for several key reasons. Firstly, it helps to uncover the underlying causes and contributing factors that lead to the perpetration of hate crimes (Analysis of hate crimes, 2024). By understanding these influences—whether they be social, economic, political, or cultural—authorities and communities can better predict when and where such crimes are likely to occur, allowing for more effective prevention measures.

Secondly, recognising the variables that drive hate crime provides a foundation for developing targeted interventions. For example, if economic hardship or political rhetoric is found to be a significant factor, strategies can be designed to address these specific issues, potentially reducing the likelihood of hate crimes occurring.

Furthermore, understanding the impact of various variables on hate crime is crucial for shaping policies and educational programmes aimed at reducing prejudice and promoting tolerance. This insight enables policymakers, educators, and community leaders to address the root causes of hate, rather than just its symptoms, fostering long-term societal change.

Ultimately, identifying these variables not only aids in reducing the incidence of hate crime but also contributes to creating a more just and inclusive society, where all individuals feel safe and valued.


## Methods

### Data Collection

### Source
This project uses reported Hate Crime data from 1991 to 2022, which has been sourced from FBI public data sets **(FBI 2023)**. To complement this, data on periods of social unrest in the United States within the same timeframe has been collected, primarily gathered from Wikipedia **(Wikipedia 2024)**.

### Variables
Key variables in the hate crime data include the data of the incident, the type of offense committed, the geographic location of the crime, and a description of the bias or motivation behind the act.

In the social unrest data, essential variables include the date of the unrest, a description of the underlying issues or biases driving the unrest, and the geographic location where the events occurred.

### Data Preparation / Cleaning

For the hate crime data (Figure 1), offence names and bias descriptions were categorised into first, second, and third level groups based on their primary characteristics, while locations were grouped into first and second level categories. Social unrest data, initially in a single column (Figure 2), was separated into year, month, type of unrest, location, and bias, with locations and biases similarly categorised. Additional cleaning and research were needed due to the public nature of the data (Figure 3).

The two datasets were merged in Excel using the COUNTIF function to display the number of incidents and social unrest events by year and month, with further breakdowns according to bias type. A preliminary visual analysis was performed using a combination chart (Figure 4). However, due to the chart's complexity, I opted to recreate the combined data, but this time aggregated by year (Figure 5). Again, a basic visual analysis was carried out using a combination chart showing no discernible trend between periods of social unrest and number of hate crimes reported.
![image](https://github.com/user-attachments/assets/b6994143-77c5-4e04-bc66-c0eb95037d45)
Figure 1. Hate crime data frim FBI with aggregations

![image](https://github.com/user-attachments/assets/29090811-4cb4-4eb5-9296-e608c00d16d4)
Figure 2. Social unrest data copied straight from Wikipedia

![image](https://github.com/user-attachments/assets/e0e75cca-fa8c-4890-8a23-2f3be816bc84)
Figure 3. Social unrest data aligned to fields with missing data inputted

![image](https://github.com/user-attachments/assets/9cbca54b-6377-446e-adc5-13641446d915)
Figure 4. Month comparison trend

![image](https://github.com/user-attachments/assets/faf7f5ea-5f28-4f79-94a7-c4b50a7b6a96)
Figure 5. Year comparison trend

![image](https://github.com/user-attachments/assets/9f24ba11-f3b0-4e18-95ed-38c6576c7738)
Figure 6. Monthly incident figures with 12-point moving trendline and 6-point polynomial trendline

![image](https://github.com/user-attachments/assets/53d46ab1-2e93-41f6-92ab-b1b2bfec45a9)
Figure 7. Scatter plot showing fitted incidents aligning with 12-point moving trendline

![image](https://github.com/user-attachments/assets/31f810c3-12ed-4f08-ad8d-fa7748a75ba7)
Figure 8. Number of incidents and Yes/No for Social Unrest where Yes = 1, No = 0

## Data Analytics

### Techniques Used
To investigate the relationship between social unrest and reported hate crimes, I employed Interrupted Time Series Analysis (ITSA) alongside the Linear Forecasting formula. ITSA will assess changes in hate crime trends during periods of unrest, while the forecasting formula will use linear regression to calculate future values. Combined, these methods will provide a comprehensive understanding of the impact of social unrest on hate crime rates and offer a monthly prediction of the overall trend.

### Justification of Methods
ITSA is employed to assess the impact of an intervention or event at a specific point in time on a time series. It does so by comparing the pre-intervention trend with the post-intervention trend, estimating the baseline before the intervention, analysing the immediate change following the intervention, and examining any change in trend (slope) thereafter.
Forecast.linear is used to predict future values in a linear trend based on existing data, assuming a linear relationship between time points and observed values.
ITSA assumes the time series is stationary around the intervention point, meaning no underlying trend should confound the results. Additionally, it must account for autocorrelation to avoid biased estimates.
Forecast.linear assumes a linear relationship between the dependent and independent variables, which may not always hold true, limiting its applicability for more complex time series. It also does not provide insights into causal relationships or the impact of interventions.


## Results

![image](https://github.com/user-attachments/assets/29e2f811-707a-48d5-b7ab-cffdf383ca97)
Figure 9. Regression summary output

The analysis demonstrates a highly statistically significant result, with only a 0.39% likelihood that the findings could be attributed to chance, indicating strong confidence in the reliability of the data. However, despite this statistical significance, the study did not identify a direct correlation between periods of social unrest and the number of reported hate crimes. This lack of direct correlation suggests that while social unrest may play a role, it is not the sole or primary driver of changes in hate crime reporting, and other underlying factors could be contributing to the variations observed during these periods.

Furthermore, an assessment of the trend in reported hate crimes since 2020 reveals a noticeable increase over time. Yet, when projecting this trend forward to 2029, the forecasted data shows only a slight increase in incidents, beginning from a lower baseline than might have been expected given the recent rise. This indicates that, although there has been an overall upward trend in hate crime reports, the projected growth in such incidents over the coming years is relatively modest. This suggests that either the recent surge in hate crimes may level off or grow at a slower rate than anticipated, providing a more tempered outlook for the future trend, or that the predictions do not show an accurate representation.

![image](https://github.com/user-attachments/assets/e924b9ef-8858-482e-b2cc-a34a0737e23a)
Figure 10. Predicted Incidents against Actual Incidents

![image](https://github.com/user-attachments/assets/39701f64-6af7-4a80-bb26-69510beda73e)
Figure 11. Actual Incidents until Dec 2022 with Predicted Incidents from Jan 2023 to Dec 2029

## Recommendations

Projecting the impact of social unrest on reported hate crimes is challenging due to several key limitations. Inconsistent data, underreporting (The Hate Crime Reporting, 2017), and differing regional practices hinder the accuracy of such projections. Establishing a direct correlation between social unrest and hate crimes is difficult because other contributing factors, such as economic stress or media influence, may also play a significant role. Moreover, timing discrepancies, regional variations, media distortion, and government interventions further complicate these projections.

Additionally, the differing short- and long-term effects of social unrest necessitate careful modelling. The challenge is exacerbated by the need to collect and integrate inconsistent data from multiple sources, where variations in data quality, reporting practices, and gaps caused by underreporting reduce reliability. These factors underscore the need for a cautious and nuanced approach to data analysis, accounting for inherent uncertainties and contextual subtleties.

During my observational analysis, I identified a significant spike in September 2001, which contributed to a notable increase in hate crimes for the entire year. This is likely linked to the aftermath of the 9/11 attacks and the subsequent rise in hate crimes and discrimination (Combating 9/11, 2015). For future research, it may be beneficial to expand the social unrest data to include external factors such as terrorism.


## Discussion and Conclusion

The ITSA model accounts for just 2.16% variance in the dependent variable, suggesting that other factors not included in the analysis may explain the remaining variance. While the significant predictors indicate that some variables have a notable influence on the dependent variable, others appear to have little impact. To enhance the model’s explanatory power, it would be beneficial to incorporate additional relevant predictors, considering transforming variables, or exploring non-linear relationships.

As an innovative approach to analysing and predicting hate crimes, this project has provided valuable insights into the factors that may be driving the rise in hate crimes within the United States. However, given the challenges in establishing a direct link between social unrest and hate crimes, it would be advantageous to include additional variables such as economic stress, media influence, and external factors like terrorism in future analyses. Additionally, a related project could examine the evolution of reporting practices, taking into account the relationship between victims and the police force. This could offer a more comprehensive understanding of the factors influencing both the incidence and reporting of hate crimes.


## References
1.	FBI Hate Crime Data Set, 2023, [online] Available [CDE(cjis.gov)](https://cde.ucr.cjis.gov/LATEST/webapp/#/pages/downloads#datasets) [Accessed June 2024]
2.	Wikipedia List of Civil Unrest, 2024, [online] Available: [List of incidents of civil unrest in the United States - Wikipedia](https://en.wikipedia.org/wiki/List_of_incidents_of_civil_unrest_in_the_United_States#1990%E2%80%931999) [Accessed June 2024]
3.	The hate crime reporting gap & why it matters, 2017, [online] Available: [The Hate Crimes Reporting Gap & Why It Matters | Not in Our Town (niot.org) ](https://www.niot.org/cops/resources/hate-crime-reporting-gap-why-it-matters) [Accessed July 2024]
4.	Analysis of Hate Crimes in the United States, 2024, [online] Available: [Analysis of Hate Crime Rates in the United States: Statistical Modeling of Public Safety Issues Based on Socioeconomic Factors | IEEE Conference Publication | IEEE Xplore](https://ieeexplore.ieee.org/document/9636943) [Accessed July 2024]
5.	U.S. Hate Crime Investigation Rates and Characteristics, 2021, [online] Available: [U.S. Hate Crime Investigation Rates and Characteristics: Findings from the National Hate Crime Investigations Study (NHCIS) (ojp.gov)](https://www.ojp.gov/pdffiles1/nij/grants/304531.pdf) [Accessed July 2024]
6.	Learn About Hate Crimes, 2024, [online] Available: [Hate Crimes | United States Department of Justice | Hate Crimes | Learn More](https://www.justice.gov/hatecrimes/learn-about-hate-crimes) [Accessed June 2024]
7.	Crime type definitions, 2024, [online] Available: [Crime type definitions](https://www.met.police.uk/sd/stats-and-data/met/crime-type-definitions/) [Accessed June 2024]
8.	Designing Buildings, 2024, [online] Available: [Purpose group - Designing Buildings](https://www.designingbuildings.co.uk/wiki/Purpose_group) [Accessed June 2024]
9.	Hate Crimes Tied to Income Inequality, 2017, [online] Available:[Higher Rates of Crime Tied to Income Inequality](https://fivethirtyeight.com/features/higher-rates-of-hate-crimes-are-tied-to-income-inequality/) [Accessed June 2024]
10.	Causes and Motivations of Hate Crime, 2016, [online] Available: [Causes and Motivations of Hate Crime](https://www.equalityhumanrights.com/sites/default/files/research-report-102-causes-and-motivations-of-hate-crime.pdf)) [Accessed June 2024]
11.	Psychological Effects of Hate Crime, 2023, [online] Available: [Psychological Effects of Hate Crime](https://www.apa.org/topics/gun-violence-crime/hate-crimes) [Accessed June 2024]
12.	Combatting Post 9/11 Discrimninatory Backlash, 2015, [online] Available: [Combatting Post 9/11 Discriminatory Backlash](https://www.justice.gov/crt/combating-post-911-discriminatory-backlash-6) [Accessed August 2024]
