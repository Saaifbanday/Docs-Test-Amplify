# MANOVA
Class __"manova"__ differs from class __"aov"__ in selecting a different summary method. Function __manova__ calls aov and then add class __"manova"__ to the result object for each stratum.​

![alt text](screenshots/image120.png){ width="700" }{ border-effect="rounded" }

Multivariate ANOVA
: Omnibus multivariate tests and corresponding F and p values are provided. Follow up univariate tests are also provided.

>NOTE: BioStat Prime currently support a single independent factor
>
{style="note"}

>NOTE: BioStat Prime don't display the confidence interval in the plot of means as there are unnecessary warnings displayed. We are working with the author of the gplots package to rectify this.
> 
{style="note"}