# Loan Modelling Project
This project creates a Decision tree model to identify customers in a Bank who have a higher probability of purchasing a loan from the bank.
The project has the following features -
- Reads a file with data about the bank customers into a pandas Dataframe.
- Run various pandas dataframe functions to do statistical analysis on the data.
- Doing data preprocessing by updating values in the Experience column which had negative values by substituting it with the absolute value. The assumption being made is that the negative sign was entered by mistake.
- Doing Exploratory univariate, bivariate and multi-variate analysis on the data using various seaborn plots.
- Splitting data into train and test datasets using sklearn train_test_split.
- Using sklearns DecisionTreeClassifier to predict loan purchasing probability.
- Creating another DecisionTreeClassifier model using pre-pruning to prevent overfitting by restricting maximum depth, max leaf nodes and  restricting the minimum samples per split.
- Creating one more model using post-pruning to reduce model complexity
- Comparing score metrics for the three models and select the best model.
- Suggest recommendations for more improvements.
