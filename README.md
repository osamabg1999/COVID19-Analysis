# COVID-19 Analysis in Mexico

Authors:  Osama Bilgrami, Kanwarpal Singh, Faiq Mohd Zulkarnain, Arteen Rafiei

## Introduction
Following the tremendous challenges posed by the COVID-19 pandemic, humanity has reached an important turning point in history, compelled to investigate, and comprehend the complexities of pandemics and their far-reaching implications. As we enter an era where the possibility of future pandemics looms large, it is critical that we strengthen our readiness and response processes. To that purpose, we are doing two independent but interconnected statistical analyses that have the potential to dramatically improve our capacity to predict the consequences of such events, similar to the COVID-19 pandemic.

The fundamental goal of our analytical efforts is to reach conclusions that will allow us to delve deeper into the complex effects of pandemics on various aspects of human existence. Our primary focus is on the investigation of crucial characteristics such as age, habits, and comorbidities, which have emerged as critical determinants in the evolution and outcome of pandemics. We hope to untangle the deep link between these parameters and the trajectory of pandemic-related outcomes through careful investigation and synthesis of multiple data sources.

Our first statistical test delves into hypothesis testing. Here, we aim to determine whether individuals aged 60 and older experience a more significant impact and higher mortality rates in comparison to those aged 18 and below due to COVID. In this context, our null hypothesis asserts that there is no difference in the proportion of COVID-related deaths between individuals above 60 and those below 18, with the difference being equal to 0. Conversely, our alternative hypothesis suggests that the mean difference is greater than 0, indicating a higher impact and mortality rate among the elderly.

In our second statistical test, we focus on investigating potential associations between an individual’s number of pre-existing health conditions and various aspects of COVID. This includes examining the likelihood of testing positive for the virus and mortality. Moreover, we aim to explore how comorbidities interact with factors such as age and gender. The objective here is to unveil the relationships and dependencies that exist between these variables.

The findings of these statistical investigations are not only significant in and of themselves, but also have implications for healthcare and policy. They have the potential to serve as the foundation for developing more targeted and effective response tactics. We hope to provide vital information to government officials, healthcare professionals, and policymakers by identifying the persons most vulnerable to the negative impacts of pandemics. In doing so, we hope to give them the skills they need to make informed decisions, allocate resources wisely, and prioritize treatments for individuals who are at a higher risk than others.

## Dataset
The dataset, generously provided by the Mexican government, has been made accessible on Kaggle and has been licensed as a CC0 Public Domain License, allowing users unrestricted utilization. Translated by a Kaggle user, this semi-structured dataset boasts 1,048,576 unique rows and 21 features encompassing anonymized patient-related information, including pre-existing conditions. The data exhibit a predominantly boolean format, utilizing 0 to denote male and 1 for female. Similarly, pre-existing conditions are also encoded as boolean values, with 0 signifying an absence and 1 indicating a presence.

There are also presence of scaled data types ranging from 1 to 5, such as the COVID severity classification, contributing to the dataset’s richness. Additionally, values of 97 and 99 under any feature serve as indicators of missing data. This comprehensive dataset thus presents a valuable resource for researchers and data enthusiasts alike, offering insights into the intricate landscape of patient profiles and health conditions in the Mexican context.

## Data Wrangling and Analysis
Please refer to the RMD file attached.

## Conclusion
The findings from both traditional proportion tests and bootstrap methods indicate that individuals aged 60 and above have a significantly higher mortality rate due to COVID-19 compared to individuals aged 18 and under. Both tests reaffirm the observed differences within the dataset thanks to the tight 95% confidence intervals.

Our Chi-Square tests provided insights on comorbidities and other factors of interest. With the entire dataset of around 1.5 million data points at our disposal, we were able to compute a near zero P
-value across all Chi-Square tests. Given the substantial number of data points we input into the chi-squared test, it is anticipated that it may detect some form of association between the factors, even if this association is influenced by external variables.

As anticipated, the results indeed revealed a significant link between the quantity of pre-existing health conditions and several variables, including COVID-19 test outcomes, COVID-19 severity, age, and gender. Furthermore, a noteworthy connection was established between comorbidities and the mortality rate, with mortality rates rising as the number of comorbidities increased.

To generate more realistic insights, we reproduced our studies by analyzing 500 random data points. While the majority of the results were similar to those obtained from assessments of the complete dataset, several variations led to different conclusions. Notably, our investigation indicated that severity and gender appeared to be uncorrelated with comorbidities. This finding, based on our sample approach, lends credence to the claim that it constitutes a more accurate conclusion. As we have seen, the large size of the dataset can make Chi-square tests prone to consistently identify relationships. This assumption is supported by the graphical representation, which clearly indicates independence between gender and comorbidities, as well as between comorbidities and severity. Consequently, our findings support the notion that employing a sampling approach may enhance the accuracy of Chi-square tests, particularly in contexts where the sensitivity of these tests in large datasets can inadvertently indicate relationships.

Our study underscores the profound impact of age and comorbidities on COVID-19 outcomes, emphasizing the need for targeted interventions, especially for older individuals and those with multiple diseases.

