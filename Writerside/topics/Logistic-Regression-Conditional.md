# Logistic Regression, Conditional

This function fits a conditional logistic regression model, which is similar to standard logistic regression, but incorporates a stratification variable. Common applications of this model are in matched case-control, matched cohort, and nested case-control studies. 

The output includes the number of strata used in the analysis, outcome frequency patterns within strata, various model summary statistics, parameter estimates, and odds ratios.

To analyse it in BioStat Prime user must follow the steps as given.

Steps
: __Load the dataset -> Click on the Model Fitting tab in main menu -> Select Regression -> This leads to analysis techniques, choose Logistics, Conditional -> There will appear a dialog -> Select the model name, dependent variables, Strata, estimation method and populate the formula builder in the dialog -> Finally execute the plot and visualise the output in output window.__

![alt text](screenshots/image210.png){ width="700" }{ border-effect="rounded" }

> Using Formula Builder: A Guide
>1.	To create an expression, click one of the buttons below and drag & drop variables.
>2.	Toggle the selected button's state by clicking it.
>3.	Place the cursor where user wants to insert the variable(s) and drag and drop or move it there.
>4.	Touch a button to see assistance.
>5.	The All N way button is not able to be toggled.

## Attributes

Dependent Variable
: This is the variable indicating the event for each subject, with 1 signifying an event, and 0 signifying a non-event. This variable must be numeric.

Formula Builder
: Specify the desired model terms.

Strata
: Specify the stratification variable. Can be numeric, character, or a nominal/ordinal factor.

Estimation Method
: Specify the model estimation method. The "Exact" method is the default. As long as there are not too many ways to select events within strata, this should be the option chosen. The estimation may take some time or lead to errors if many combinations can result within some strata, say 100 events out of 500 subjects. The Efron and Breslow approximations are adequate in these cases, with Efron being preferred. See the references in the R help for details.

>Required R Packages: survival, broom, arsenal, dplyr
> 
{style="note"}