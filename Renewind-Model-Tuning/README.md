# Renewind Model Tuning Project
This project uses Tensorflow Sequential model to identify a set of given data points for wind turbines which can predict failures for them early, so that they could be repaired instead of replacing bad ones which is much more costly.
The project has the following features -
- Reads a file with data points about the turbines into a pandas Dataframe.
- Run various pandas dataframe functions to do statistical analysis on the data.
- Doing Exploratory univariate, bivariate and multi-variate analysis on the data using various seaborn plots.
- Splitting data into train, validation datasets using sklearn train_test_split. The test dataset was given for the project in a separate file.
- Using sklearn SimpleImputer to fill in missing values in the split datasets, with strategy of median as those features had outliers.
- Using Tensorflow Sequential model with a layer of 128 neurons to predict breakage with sigmoid activation in the output layer. Creating multiple models and using Recall Score to compare performance of the models.
- Creating a 2nd model with one more hidden layer of 64 neurona and relu activation and got performance metrics.
- Creating a third model. Increasing momentuim to 0.7 for the SGD optimizer and reducing learning rate to .001 and got performance metrics.
- Creating a fourth model. Increasing momentuim to 0.9 for the SGD optimizer and reducing learning rate to .0001 and also changed activation for 2nd hidden layer to tanh and got performance metrics.
- Creating a fifth model. Adding one more hidden layer with 64 neurons and relu activation. Changing optimizer to Adam and got performance metrics.
- Creating a sixth model with reduced learning rate of 0.0001 for the Adam optimizer and got performance metrics.
- Creating a sixth model by adding dropout rates of 4%, 2% and 2% respectively for the hidden layers and got performance metrics.
- Creating a sixth model by using the He-normal weight initializer for all the layers along with the dropouts introduced in the previous model.
- Comparing the Recall score metrics for the  models to select the best model which turned out to be the first model.
- Suggest recommendations for more improvements.
