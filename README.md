### Machine Learning Model Descriptions
#### Description of the preliminary data preprocessing
Prior to developing the machine learning model, the data from all three datasets (Happiness, Freedom, and Life-Expectancy) was cleaned by using Pandas to drop NaNs, duplicates, and unnecessary columns and the dataframes were merged to create one final dataframe. The datatypes of columns were also changed to be input in the machine learning model and the data was split by year into 2015 and 2016 dataframes. To pre-process the data for the machine learning model, Scikit-Learn was used to define the features and target sets and to scale the data with StandardScaler.

#### Description of preliminary feature engineering and preliminary feature selection
The target, y, is meant to be the output that the machine learning model will try to predict. For this project, happiness score was selected as the target and was created by using just that column from our final dataframe. The features for our machine learning model were selected by dropping the year and all columns from the happiness dataset and using all  the other columns as features, specifically from the Life Expectancy and freedom datasets. Some trial and error was done to select features with different levels of correlation with the target, but the best results came from using all columns other than those originally used to determine the happiness score in the happiness dataset.

#### Description of how data was split into training and testing sets
The data was split into training and testing sets by using the 2015 data as the training data and testing on the 2016 data. These dataframes were split by year from the original merged dataframe. This method produced a much higher accuracy score compared to using Scikit-Learn's train_test_split on the whole merged dataset.

#### Explanation of model choice, including limitations and benefits.
For our data, our group chose to use a supervised linear regression machine learning model to predict the happiness score of a country based on the features in the dataset. The benefits of using a linear regression model are that it will be able to predict the happiness score, a continuous variable,  based on the features of the data. A limitation of the linear regression model is that is assumes a linear relationship between the features and target and could miss some outliers or actual results that are not directly correlated.

#### Model Training
The training for the linear regression model was conducted using the 2015 data, with the features selected as described above, to train the model to be tested with the 2016 data. Future iterations of training the model can be done by changing the training parameters and/or changing the model features to include different columns, such as those with a high correlation to the happiness score.

#### Description of Current Accuracy Score
Our machine learning model uses the sklearn r2_score, coefficient of determination, to assess the accuracy of the model. The current r2 score is 71.7%, which reveals that nearly 72% of the predicted data fits the linear regression model. This current accuracy score can be improved upon but is fairly accurate, especially compared to alternate models that were tested using sklearn's train-test-split and received accuracy scores of under 45%.
