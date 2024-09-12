# Cox, Fine-Gray

Fits a Fine-Gray Cox proportional hazards model for time-to-event data with censored observations when competing risks are present. Fine-Gray models model the effect of covariates on the cumulative incidence function. 

An alternative is to model the effect of covariates on the cause-specific hazard, for which standard Cox regression models can be used.

To analyse it in BioStat Prime user must follow the steps as given.

Steps
: __Load the dataset -> Click on the Model Fitting tab in main menu -> Select Regression -> This leads to analysis techniques, choose Cox, Fine-Gray -> There will appear a dialog -> Select the variables in the dialog and populate a formula -> Finally execute the plot and visualise the output in output window.__

![alt text](screenshots/image198.png){ width="700" }{ border-effect="rounded" }

## Attributes

Enter model name
: Specify the name of the model where the results will be stored.

Time to event or censor
: Time to the first event for those experiencing an event or time to last follow-up for those not experiencing any event

Events (0 = censor, 1 = event 1, 2 = event 2, ...)
: Numerical event indicator; 0=censor, 1=event 1, 2=event 2, etc.

Event Code
: Select the event of interest you want to model. Can either be selected or typed in.

Formula Builder
: Construct terms to include in the model. Factors, strings, and logical variables will be dummy coded. The provided buttons allow user to specify main effects, full factorial effects (main effects and all interactions with the involved variables), polynomials, specific interactions, and delete terms from the list. Interactions with stratification variables is allowed.

Stratification Variables
: Specify one or more stratification variables. These can be numeric, factor, ordered factor, or character variables. The strata divide the subjects into separate groups whereby each group has a distinct baseline hazard function. If multiple stratification variables are given, a separate baseline hazard function is used for every combination of stratification variable levels.

Weights
: Numeric variable for observation weights. Useful in situations where each record should not be counted as one observation.

## Options

Tied Time Method
: Method of breaking tied observed times. Efron is usually the better choice when there aren't many tied times.

Model Diagnostics
: If selected, an assessment of proportional hazards and functional form of covariates will be assessed, including relevant plots. If there are stratification variables or non-numeric predictors, functional form plots will not be produced. The Null Model Martingale Residual Axis Minimum Value might need to be changed in order to see all Martingale residuals.

Analysis of Deviance (Type II)
: If selected, whole variable tests (including multi-degree of freedom tests for multi-category covariates) will be provided. Wald tests are used.

>Required R packages: survival, broom, survminer, car, dplyr
>
{style="note"}

> The model is fit using the finegray and coxph functions in the survival package.
> 
{style="note"}

>Click the R Help button to get detailed R help about the coxph function. Go to Help-> R Function Help to get more information about the finegray function, which creates the needed dataset.
> 
{style="note"}