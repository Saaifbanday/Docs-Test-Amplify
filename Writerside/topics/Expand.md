# Expand

Creates a new dataset with rows expanded as per weights. In this dialog the weights refer to the dataset variable that contains the weights.

To expand weights user needs to follow the steps given bellow.

Steps
: __Load the dataset -> Click on the DATASET tab in main menu -> select EXPAND -> Once the dialog appears choose the Variable to be expanded -> Execute the dialog.__

![Expand](screenshots/Expand.png){ width="700" }{ border-effect="rounded" }

Before expanding weights.

![Before expanding](screenshots/Expand Before expanding.png){ width="700" }{ border-effect="rounded" }

![Expand Before expanding](screenshots/Expand Before expanding2.png){ width="700" }{ border-effect="rounded" }

After Expanding weights.

![Expand After Expanding](screenshots/Expand After Expanding.png){ width="700" }{ border-effect="rounded" }

![Expand After Expanding](screenshots/Expand After Expanding2.png){ width="700" }{ border-effect="rounded" }

The arguments used is executing the dialog are given as follows.

{type="full"}
Arguments
:
1. Weights: The dataset variable that contains the weights.
2. data: The input data.frame or data.table.
3. newdata: The new dataset where the rows are replicated for the weights specified.