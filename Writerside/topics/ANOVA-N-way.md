# ANOVA, N way

Fits an analysis of variance model, displays type I,II,III sum of squares, displays marginal means and contrasts (using marginal means).

>Optionally performs Levene's test for homogeneity of variance across groups and plots graphs.

>Levene's test is run for all the main effects
>
{style="note"}

In statistics, an N-way ANOVA (Analysis of Variance) with blocks refers to a statistical analysis that involves multiple independent variables or factors (more than two). The term "blocks" in this context refers to __a way of handling potential sources of variability__ that are not the primary focus of the study but need to be accounted for to improve the precision of the analysis. 

N-way ANOVA indicates that there are multiple independent variables (factors). For example, in a 2-way ANOVA, there are two independent variables, and in an N-way ANOVA, there are more than two. Each independent variable can have multiple levels or categories. 

>N-way ANOVA with blocks involves analyzing the effects of multiple independent variables on a dependent variable while taking into account the potential impact of blocking variables.

To analyse it in BioStat Prime user must follow the steps as given.
Steps
: __Load the dataset -> Click on the analysis tab in main menu -> Select means The means tab leads to the ANOVA, N way analysis technique in the dialog -> In the dialog select the target variable and create a formula according to the requirement -> Execute the dialog.__

![ANOVA, N way](screenshots/ANOVA N way.png){ width="700" }{ border-effect="rounded" }

>NOTE:
>1. To get all marginal means and post-hocs user needs to construct a formula with the main effects and all the interaction terms in the model.
    So if you are attempting to analyze a 3 way interaction, user needs to specify     
    __A + B + C + A:B + B:C + A:C + A:B:C__       
    If instead you specify A*B*C, user will get the complete ANOVA table, user will NOT get the estimated marginal means and post-hocs for all the interactions.
>2. Estimated marginal means AND POST-HOCS are computed for all main effects and the SPECIFIED INTERACTIONS

The user can build a formula in the formula builder by following the steps given below.

>1.	Click on a button in formula builder and drag and drop variables to create an expression.
>2.	Clicking a selected button will toggle its state.
>3.	To insert at a position, place the cursor in that position and drag & drop/move variable(s).
>4.	Mouse over a button for help.
>5.	User cannot toggle the All N way button.