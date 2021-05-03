Team members submit the code for 
their machine learning model, as well 
as the following:

### Description of the preliminary data preprocessing
Prior to developing the machine learning model, the data from all three datasets (Happiness, Freedom, and Life-Expectancy) was cleaned by using Pandas to drop NaNs, duplicates, and unnecessary columns and the dataframes were merged to create one final dataframe. The datatypes of columns were also changed and the columns with data as text were one-hot encoded. To pre-process the data for the machine learning model, Scikit-Learn was used to define the features and target sets, split the data into training and testing data using train_test_split, and to scale the data with StandardScaler.

### Description of preliminary feature engineering and preliminary feature selection
The target, y, is meant to be the output that the machine learning model will try to predict. For this project, happiness score was selected as the target and was created by using just that column from our final dataframe. The features for our machine learning model were selected by dropping the target (happiness score) from the final dataframe and using every other column.

### Description of how data was split into training and testing sets
Write Description of how data was split into training and testing sets here.

### Explanation of model choice, including limitations and benefits.
Write an explanation of model choice, including limitations and benefits here.

