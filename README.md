Team members submit the code for 
their machine learning model, as well 
as the following:

### Description of the preliminary data preprocessing
Prior to developing the machine learning model, the data from all three datasets (Happiness, Freedom, and Life-Expectancy) was cleaned by using Pandas to drop NaNs, duplicates, and unnecessary columns and the dataframes were merged to create one final dataframe. The datatypes of columns were also changed and the columns with data as text were one-hot encoded. To pre-process the data for the machine learning model, Scikit-Learn was used to define the features and target sets, split the data into training and testing data using train_test_split, and to scale the data with StandardScaler.

### Description of preliminary feature engineering and preliminary feature selection
The target, y, is meant to be the output that the machine learning model will try to predict. For this project, happiness score was selected as the target and was created by using just that column from our final dataframe. The features for our machine learning model were selected by dropping the target (happiness score) from the final dataframe and using every other column.

### Description of how data was split into training and testing sets
Scikit-Learn's train_test_split function was used to split the data into random training and testing datasets (X_train, X_test, y_train, y_test) with a random_state of y and stratified.

### Explanation of model choice, including limitations and benefits.
For our data, our group chose to use a supervised linear regression machine learning model to predict the happiness score of a country based on the features in the dataset. The benefits of using a linear regression model are that it will be able to predict the happiness score, a continuous variable,  based on the features of the data. A limitation of the linear regression model is that is assumes a linear relationship between the features and target and could miss some outliers or actual results that are not directly correlated.
