# Context

The data set we will be working with contains information on various cars. 
For each car we have information about the technical aspects of the vehicle such as the motor's 
displacement, the weight of the car, the miles per gallon, how fast the car accelerates, and more. 

The dataset is included in the `imports-85.data` file.

# Objective

We will be using K-Nearest Neighbors algorithm that predicts car prices & figure out the best k_neighbors to use to optimize the model.

# Process

First, we explore the data and clean the columns.
We fill any null values with the mean or the most common value in the column.
We also normalize all numerical columns to avoid certain columns being weighted differently in the algorithm.

We create an univariate model by iterating over each feature with different `n_neighbors`.

Then, we create a multivariate model and iterate over different number of features with different `n_neighbors`.
We visualize our findings.

# Results

We use Root Mean Square Error(RMSE) as our error indicator. 
For both the univariate model and the multi variate models, the analysis suggests a low value of `n_neighbors` has the lowest RMSE.
However, the algorithm might be affected by overfitting at low `n_neighbors`.
