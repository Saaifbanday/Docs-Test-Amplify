# Cox, Binary Time-depended covariates

Fits a Cox proportional hazards model for time-to-event data with censored observations that includes one or more binary time-dependent __"exposure"__ covariates. This type of covariate is one where the occurrence of a __"yes"__ can happen after the start of follow-up and once that __"yes"__ occurs it stays a __"yes"__ for the follow-up duration. An example would be rejection of a graft post-transplant (i.e. before the rejection occurs, the patient has not been "exposed"; after rejection occurs, the patient has been "exposed"). Treating such a covariate as being known at the start of follow-up is a form of looking into the future and leads to biased estimates (also known as "immortal time bias").

To analyse it in BioStat Prime user must follow the steps as given.

Steps
: __Load the dataset -> Click on the Model Fitting tab in main menu -> Select Regression -> This leads to analysis techniques, choose Cox, Binary Time-depended covariates -> There will appear a dialog -> Select the variables in the dialog and populate a formula -> Finally execute the plot and visualise the output in output window.__

![alt text](screenshots/image197.png){ width="700" }{ border-effect="rounded" }

__Arguments__

Enter model name
: Name where the model results will be stored.

Time to event or censor
: Time to outcome event for those experiencing the event or time to last follow-up for those not experiencing the outcome event.

Events (1=event, 0=censor)
: Numerical event indicator; 1=event, 0=censor.

Formula Builder
: Construct terms to include in the model. Factors, strings, and logical variables will be dummy coded. The provided buttons allow user to specify main effects, full factorial effects (main effects and all interactions with the involved variables), polynomials, specific interactions, and delete terms from the list.

Exposure time variables for time-dependent covariates
: Numeric variables storing the time when the subject was first "exposed". This must be on the same time scale as the Time variable. Missing values should be used for subjects who were never exposed. Each variable specified here will create a separate time-dependent covariate. A specified time assumes that a subject is not exposed prior to this time and exposed after this time (i.e. when the predictor change from "no" to "yes"). Specifying only positive values means that subjects are not exposed for some time after follow-up starts. Specifying some positive and negative times indicates that some subjects were exposed after and some before follow-up time starts, respectively. If user knows that a subject was exposed prior to the follow-up start time, but user doesn't know exactly when, then user can use any negative time and the model will correctly treat that subject as being exposed for their entire follow-up time. If subjects are exposed after follow-up, then they are correctly treated as not being exposed for their entire follow-up time.

Prefix for time-dependent covariates
: Desired prefix to be used for every time-dependent covariate specified in the Exposure time variables field. The name of each time-dependent covariate will start with this prefix.

Subject identifier
: The variable storing the subject identifier. This is required for purposes of creating the underlying counting process data set.

Weights
: Numeric variable for observation weights. Useful in situations where each record should not be counted as one observation.

### Options
Model fitting statistics, parameter estimates, and hazard ratios are provided. Options available include the tied time method, forest plots, model diagnostics, and the ability to view the underlying counting process data set that gets created.

#### Tied Time Method:
Method of breaking tied observed times. Efron is usually the better choice when there aren't many tied times. The exact method can be beneficial if there are many tied times, as in discrete time situations, but can take a little longer for the model to be fit.

#### Forest Plot: 
Will create a forest plot of hazard ratios and confidence intervals

#### Show (start, stop) Data Set: 
Will show the underlying counting process data set used in the computations. This breaks each subject's follow-up time into parts, depending on when the time-dependent covariate should change values.

#### Model Diagnostics: 
If selected, proportional hazards tests and plots will be provided, in addition to assessments of functional form for each covariate in the model. The null model Martingale residual axis minimum value option might need to be changed so that all residuals appear in the plot. To get functional form assessments, you must specify only numeric predictors and have no missing data. See Variables > Missing Values > Remove NAs.

#### Analysis of Deviance (Type II): 
Global test of each predictor in the model. Multi-degree of freedom tests will be provided for effects with more than 2 levels. Wald and Likelihood ratio tests can be obtained, with likelihood ratio tests having better small sample properties.

>The model is fit using the `coxph` function in the survival package.
> 
{style="note"}