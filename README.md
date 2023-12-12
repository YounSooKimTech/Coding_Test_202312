# Name: Joy Kim (yk2949)

## Objective
This simulation aimed to investigate whether appeals based on reason or emotion influence people's perceptions and behaviors regarding COVID-19 vaccination, compared to a control group.

## Data
Simulated data, located in the Data folder, includes demographic variables (age, sex, ethnicity, education level, flu vaccination history, and living area) based on American Community Survey data. 
The demographic variables tried to resemble the American Community Survey Dataset. 
For instance, random assignment was conducted with a 7:3 ratio for a university degree. 
Perception was measured on a 1-5 Likert scale before and after exposure to ads.
Behavior was coded as 0 (not vaccinated) or 1 (vaccinated) for getting vaccination within one year. 

## Participants
A total of 4500 participants from the 5000 baseline dataset were selected for the endline survey. 
Random assignments were evenly distributed across control (1689), emotional appeal (1675), and reason appeal (1636) groups.

## Data Processing
Character variables were dummy coded with a prefix of D_ for convenience. 
A check for randomization quality showed weak Pearson correlations among variables, confirming the randomness of assignments.

## Graphs
Graphs illustrate the perception before and after exposure to ads in each group and the proportion of vaccinated individuals within one year. 
Before ad exposure, no statistically significant differences were expected. 
Post-ad exposure, emotional and reason appeals were anticipated to positively impact COVID-19 vaccination perceptions and increase vaccination rates compared to the control group.

## Statistical Tests
ANOVA for perception before and after ads differences yielded a statistically insignificant result (F(2, 4497) = 2.41, p = 0.09). 
Post-hoc Tukey tests showed no significant mean differences between different ad exposure groups and the control group.

Logistic regression, coding vaccination as 1 (vaccinated within one year) or 0 (not vaccinated within one year), revealed that only the reason appeal experimental group had a significant p-value (< 0.05). 
The beta coefficient for the reason experimental group was 0.15, suggesting a 16% higher likelihood of vaccination within one year compared to the control group when controlling for other variables.

## Suggestions
Due to computing resource limitations, repeated ANOVA in R was not conducted. 
Future studies could benefit from exploring before-and-after differences using repeated measures analysis. 
Additionally, consider including other influential variables, such as living area. 
Based on findings from previous studies, residing in an urban area was associated with a twofold increase in vaccination rates. 
Therefore, these demographic variables should be considered as covariates in the future analysis.

## References
- Saelee, R., Zell, E., Murthy, B. P., Castro-Roman, P., Fast, H., Meng, L., ... & Murthy, N. (2022). Disparities in COVID-19 vaccination coverage between urban and rural counties—United States, December 14, 2020–January 31, 2022. Morbidity and Mortality Weekly Report, 71(9), 335.

- Lomeli, A., Escoto, A. A., Reyes, B., Burola, M. L. M., Tinoco-Calvillo, S., Villegas, I., ... & Seifert, M. (2023). Factors associated with COVID-19 vaccine uptake in a US/Mexico border community: demographics, previous influenza vaccination, and trusted sources of health information. Frontiers in Public Health, 11.





