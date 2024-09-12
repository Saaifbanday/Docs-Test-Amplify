# Linear Regression (Legacy)

To analyse it in BioStat Prime user must follow the steps as given.

Steps
: __Load the dataset -> Click on the Model Fitting tab in main menu -> Select Regression -> This leads to analysis techniques, choose Linear, Basics(Legacy) -> There will appear a dialog -> Select the model name, dependent variables and independent variable in the dialog -> Check the radio buttons to display a plot in the output -> Finally execute the plot and visualise the output in output window.__

![alt text](screenshots/image205.png){ width="700" }{ border-effect="rounded" }

![alt text](screenshots/image206.png){ width="700" }{ border-effect="rounded" }

## Arguments

depVar
: Name of the dependent variable. If we have a dataset cars, with a variable mpg that we want to predict mpg (dependent variable is mpg) enter mpg

indepVars
: Names of the dependent variable. If we have a dataset cars, with dependent variable horsepower, enginesize, enter horsepower+enginesize. Categorical variables are automatically dummy coded.

dataset
: Name of the dataframe. When you open data frames or datasets e.g. csv, Excel files, SAS files in BioStat Prime, they are named Dataset1, Dataset2, Dataset3 so enter Dataset1