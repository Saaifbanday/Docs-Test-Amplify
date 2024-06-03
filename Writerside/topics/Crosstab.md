# Crosstab

In statistics, a crosstab, short for "cross-tabulation," is a table that displays the relationships between two or more categorical variables. It provides a summary of the distribution of one variable in relation to another. Crosstabs are particularly useful for analyzing and visualizing the association or dependency between categorical variables. Crosstabs are used when both variables under consideration are categorical. Categorical variables have distinct categories or groups with no inherent order. The chi-square test of independence is often used in conjunction with crosstabs to determine whether there is a statistically significant association between the variables. This test assesses whether the observed frequencies in the cells are significantly different from what would be expected if the variables were independent. BioStat Prime lays out 3 options in its Crosstab tab, i.e.

### Crosstab

The main purpose of a crosstab is to show the frequency distribution of one variable across the levels of another variable.

To analyse it in BioStat Prime user must follow the steps as given.

__Load the dataset -> click on the analysis tab in main menu -> select Crosstab -> TheCrosstab contains 3 options, select the first one namely crosstab -> This leads to the crosstab analysis technique in the dialog -> Select the row and column variables -> Execute the dialog.__

![alt text](screenshots/image99.png){ width="700" }{ border-effect="rounded" }

The result of the analysis will be visible in the output.When multiple row and column variables are specified, a separate cross table for each pair of row and column variables is generated.

### Crosstab List

In addition to raw counts, crosstabs often include percentages. These can be row percentages (percentage within each row) or column percentages (percentage within each column).

To analyse it in BioStat Prime user must follow the steps as given.

__Load the dataset -> click on the analysis tab in main menu -> select Crosstab -> The Crosstab contains 3 options, select the second one namely crosstab list -> This leads to the crosstablist analysis technique in the dialog -> Select variables for the table -> Execute the dialog.__

![alt text](screenshots/image100.png){ width="700" }{ border-effect="rounded" }

User can also opt for other options at the bottom related to frequencies, include combinations with 0 counts, show top N most frequent values.

### Odds Ratio/ Relative Risks, M by 2 Table

When working with a crosstab (contingency table) that involves categorical variables, measures such as odds ratios, relative risks, and the chi-square test (often referred to as the "chi-square test of independence") are commonly used to assess associations between variables.

The odds ratio is a measure of association between two binary variables. It is commonly used in case-control studies or situations where the outcome is dichotomous. The odds ratio indicates the odds of an event occurring in one group relative to the odds in another group.

The relative risk (RR) is another measure of association, commonly used in cohort studies or situations where the outcome is binary.The relative risk indicates the risk of an event occurring in one group relative to the risk in another group.

The chi-square test is used to assess whether there is a statistically significant association between two categorical variables. The test involves comparing the observed frequencies in a contingency table with the frequencies that would be expected under the assumption that the variables are independent .A significant chi-square test suggests that the variables are associated.

The choice between odds ratio and relative risk depends on the study design and the nature of the data. Chi-square test is used to determine whether observed associations are statistically significant.

![alt text](screenshots/image101.png){ width="700" }{ border-effect="rounded" }

To analyze all three of them in BioStat Prime user must follow the steps as given.

__Load the dataset -> Click on the analysis tab in main menu -> Select Crosstab -> TheCrosstab contains 3 options, select the third one namely Odds Ratio/ Relative Risks, M by 2 Table -> This leads to the crosstablist analysis technique in the dialog -> Select variables for the table -> Execute the dialog.__
