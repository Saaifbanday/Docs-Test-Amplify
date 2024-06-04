# Distribution Analysis

In statistics, a distribution refers to the set of all possible values and their corresponding probabilities or frequencies for a given variable. Understanding the distribution of data is fundamental in statistical analysis. Different statistical tests can be employed to assess whether a given dataset follows a specific distribution, such as the normal distribution. BioStat Prime brings forth some normality distribution tests under the distribution sub menu in analysis tab of main menu. The distribution tab comprises 7 normality test that are discussed below in detail. Users must keep in mind that normality tests are sensitive to sample size, and with large sample sizes, even small departures from normality may lead to rejecting the null hypothesis. It's essential to consider the context of your data and the specific requirements of user’s analysis when interpreting the results of normality tests.

### Anderson-Darling Normality Test

The Anderson-Darling test is one such test, and it is specifically used for testing the goodness of fit of a sample to a specified distribution, often the normal distribution. The Anderson-Darling test is more sensitive to deviations in the tails of the distribution compared to other normality tests like the Shapiro-Wilk test.

To analyse it in BioStat Prime user must follow the steps as given.

__Load the dataset -> click on the analysis tab in main menu -> select Distribution tab -> The Distribution tab contains 7 options, select the first one namely Anderson-Darling Normality test -> This leads to analysis technique in the dialogselect variables to target -> Execute the dialog.__

![alt text](screenshots/image102.png){ width="700" }{ border-effect="rounded" }

### Kolmogorov-Smirnov Normality Test

The Kolmogorov-Smirnov (K-S) test for normality is a non-parametric test used to determine whether a sample comes from a normal distribution. It is based on the cumulative distribution function (CDF) of the normal distribution and involves comparing the observed cumulative distribution of the data with the expected cumulative distribution of a normal distribution. The Kolmogorov-Smirnov test is sensitive to departures from normality in both the center and the tails of the distribution. When the sample size is small, the test may have limited power to detect deviations from normality.

To analyse it in BioStat Prime user must follow the steps as given.

__Load the dataset -> Click on the analysis tab in main menu select Distribution tab -> The Distribution tab contains 7 options, select the second one namely Kolmogorov-Smirnov Normality test -> This leads to analysis technique in the dialog -> Select variables to target -> Execute the dialog.__

![alt text](screenshots/image103.png){ width="700" }{ border-effect="rounded" }

### Shapiro-Wilk Normality Test

The Shapiro-Wilk test is a statistical test used to assess whether a sample comes from a normally distributed population. It is commonly used for testing the assumption of normality in statistical analyses. The test is particularly useful when dealing with smaller sample sizes.The Shapiro-Wilk test is sensitive to deviations from normality, especially in the tails of the distribution.

To analyse it in BioStat Prime user must follow the steps as given.

__Load the dataset -> click on the analysis tab in main menu -> Select Distribution tab -> The Distribution tab contains 7 options, select the third one namely Shapiro-Wilk Normality Test -> This leads to the analysis technique in the dialog -> Select variables to target -> Execute the dialog.__

![alt text](screenshots/image104.png){ width="700" }{ border-effect="rounded" }

### Distribution Fit

Distribution fitting is a statistical technique used to model and describe the distribution of a dataset by finding the probability distribution that best fits the observed data. The goal is to identify a parametric distribution (such as normal, exponential, gamma, etc.) that provides a good representation of the data.

To analyse it in BioStat Prime user must follow the steps as given.

__Load the dataset -> Click on the analysis tab in main menu -> Select Distribution tab -> The Distribution tab contains 7 options, select the fifth one namely Distribution Fit -> This leads to the analysis technique in the dialog -> Select variables to target -> Fit the test for various distributions -> Execute the dialog.__

![alt text](screenshots/image105.png){ width="700" }{ border-effect="rounded" }

The various distributions in the output window.

![alt text](screenshots/image106.png){ width="700" }{ border-effect="rounded" }

### Distribution Fit with Gamlss

The Gamlss package in R is used for fitting Generalized Additive Models for Location, Scale, and Shape (GAMLSS). GAMLSS is a flexible framework for modeling distributions and is capable of handling a wide range of distributional shapes. BioStat Prime utilizes this package of R to aids user to fit different parametric gamlss.family distributions from R pkg gamlss.

To analyse it in BioStat Prime user must follow the steps as given.

__Load the dataset -> click on the analysis tab in main menu select Distribution tab -> The Distribution tab contains 7 options, select the sixth one namely Distribution Fit with Gamlss -> This leads to the analysis technique in the dialog -> Select variables that contains distribution -> Check the options at the bottom as per the preference -> Execute the dialog.__

![alt text](screenshots/image107.png){ width="700" }{ border-effect="rounded" }

### Distribution Analysis Cullen and Frey Graph

The Cullen and Frey graph, also known as the Cullen and Frey graph for skewness and kurtosis, is a graphical method for assessing the skewness and kurtosis of a dataset. It's a visual tool that helps you quickly inspect the departure from normality in terms of skewness and kurtosis. BioStat Prime aids users to derive Cullen and frey graph with descriptive of an empirical distribution of a non-censored data.

To analyse it in BioStat Prime user must follow the steps as given.

__Load the dataset -> click on the analysis tab in main menu -> Select Distribution tab -> The Distribution tab contains 7 options, select the seventh one namely Distribution Analysis Cullen and Frey Graph -> This leads to the analysis technique in the dialog -> Select variables that contains distribution -> Check the options at the bottom as per the preference -> Execute the dialog.__

![alt text](screenshots/image108.png){ width="700" }{ border-effect="rounded" }
