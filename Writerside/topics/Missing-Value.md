# Missing Value

#### Column layout

To analyse it in BioStat Prime user must follow the steps as given.

Steps
: __Load the dataset -> Click on the analysis tab in main menu -> Select missing values -> The missing values tab leads to column layout in the dialog -> Execute the dialog.__

![alt text](screenshots/image124.png){ width="700" }{ border-effect="rounded" }

#### Row layout

Missing value analysis is an essential step in data preprocessing, helping you understand and handle missing data in your dataset. The "row layout" in this context suggests that user is examining missing values on a row-wise basis, looking at how missing values are distributed across individual rows in user's dataset.

Analyzes missing values and displays results in rows, displays summary information of missing values at the variable level and lists the number of missing values on each row for variables being analyzed.

Provides a summary for each variable of the number, percent missings, and cumulative sum of missings of the order of the variables. By default, it orders by the most missings in each variable.

To analyse it in BioStat Prime user must follow the steps as given.

Steps
: __Load the dataset -> Click on the analysis tab in main menu -> Select missing values -> The missing values tab leads to row layout in the dialog -> In the dialog select the variable and options according to the requirement -> Execute the dialog.__

![alt text](screenshots/image125.png){ width="700" }{ border-effect="rounded" }

>Arguments

data
: a dataframe

order
: a logical indicating whether to order the result by n_miss. Defaults to TRUE. If FALSE, order of variables is the order input.

add_cumsum
: logical indicating whether or not to add the cumulative sum of missings to the data. This can be useful when exploring patterns of nonresponse. These are calculated as the cumulative sum of the missings in the variables as they are first presented to the function.