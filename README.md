#### Description of the source of data
The main dataset being used is a collection of data from the [World Happiness Report](https://www.kaggle.com/unsdsn/world-happiness). It is a landmark survey of the state of global happiness. The data set has a collection of indicators on more than **140 countries** around the world including happiness rank, happiness score on a scale of 0 to 10, standard error, and more… The data set includes reports from 2015 to 2019. 

We will also be using the [World Bank Life Expectancy](https://data.worldbank.org/indicator/SP.DYN.LE00.IN) data set and the [Human Freedom Index](https://www.kaggle.com/gsutters/the-human-freedom-index), to compare against (for the years that align with our main data set). 

#### Questions they hope to answer with the data
We want to find which factors influence happiness within a country and we would also like to foind out how to predict the happiness scores, if it is at all possible to do so.

### Decision Log

A decision will also be used and updated, to showcase and record point of consensus:

| Date Recorded | Decision Description |
| ------------- | ------------- |
| 20 Apr 21  | Final project topic to be about **Happiness**. Selected [World Happiness Report](https://www.kaggle.com/unsdsn/world-happiness) has the main database for the project |
| 22 Apr 21  | Responded, as a team, to *Presentation* topics |
| 22 Apr 21  | Team decided to find correlation between life expectancy, general sense of freedom, and its effect on a country happiness |
| 22 Apr 21   | Team decided to use multiple dataset (focusing on 2018 and 209 for now) to compare World Happiness Report database with life expectency and Human Freedom Index   |
| 23 Apr 21   | Diana created the list of technologies to use for Segment I|
| 23 Apr 21  | Assitan dveloped ERD |
| 25 Apr 21  | Team merged deliverables onto the main branch (ERD, Database, Mockup Machine learning, Technology to be used) |
| 29 Apr 21  | Used pgAdmin 4 to create a database using our 3 dataset |
| 29 Apr 21  | Modified Final_Project Machine_Learning Mock_up.ipynb file to connect to database |
| 09 May 21  | Completed most deliverables and focusing on presentation. Need to control main branch submissions |


#### Risk and Issue Management

This team recognize that risk and issue may arise trough the course of our collaboration. The team has listed below potential problems that might arise during the project, their causes, symptoms, consequences, and possible solutions.

| Date Recorded | Risk Description | Probability | Impact | Mitigation Plan |
| ------------- | ------------- | ------------- | ------------- | ------------- |
| 22 Apr 21  | Choosing a database that provides a poor machine learning output  | Medium | High  | Consulting TAs to guide us at each step of the process |
| 22 Apr 21  | A team member feeling overworked or underworked  | Medium  | Medium  | For each segment, the team agrees to a breakdown of the deliverables and offer/receives support where needed   |
     

The risk register above will be periodically updated to list any issue that may have come up. For high propability and high impact issue that have no mitigation in place, the team will:

![Risk Escalation Process](https://github.com/GloriaY007/Final-Group-Project-/blob/GloriaY-S/Risk%20Ecalation%20Process.png)

### Segment I: Sketch It Out!

During the 1st Segment,  ***The Ladies*** project team, will be focused on outlining the structure of the overall group project. During this phase, Gloria will be a :black_square_button:, Lynn will be a :small_red_triangle:, Assitan will be a :red_circle:, and Diana will be an :heavy_multiplication_x:. 

Here is a list of deliverables for *Sunday, April 25, 2021* and their assigned reponsible team member:
- [x] Topic for the project 
- [x] Read Me by @GloriaY007
     - [x] Communication Protocol
     - [x] Repository Management
- [x] Identification of technology to use by @borkard
- [x] Exploratory data analysis by @assaci
- [x] Mockup of machine learning by @lynnokang

#### Technology to be used:
##### Data Cleaning and Analysis
Pandas will be used to clean the data and perform an exploratory analysis. Further analysis will be completed using Python. Matplotlib will be used to visualize the results of our analysis. Jupyter notebook will be used throughout as the platform for analysis.

##### Database Storage
PostgreSQL is the database we will use to store our data and pgAdmin will be used as an interface to query the data. The module psycopg2 will be used to connect Python with Postgres.

##### Machine Learning
SciKitLearn is the machine library we'll be using to create a classifier. We plan on using a linear regression model and either ridge regression or lasso regression. Our train-test-split will follow the default standard of 75% of the data for training and 25% for testing.

##### Dashboard
Tableau will be used to create a dashboard to display the results of our analysis. A ReadMe on GitHub will also be kept updated with all text and visuals throughout the project.


#### Exploratory Data Analysis (ERD)

##### ERD

![ERD](https://github.com/GloriaY007/Final-Group-Project-/blob/Assitan_C/ScreenShots/ERD.png?raw=true)

##### Database Storage Set Up 
PostgreSQL will be used for database storage. 
- Happiness RDS instance was already set up in ASW.The database was made public so everyone can have access.
- A new server happiness and a database Final_ Project were created on PostgreSQL. 

![AWS](https://github.com/GloriaY007/Final-Group-Project-/blob/Assitan_C/ScreenShots/AWS.PNG?raw=true)


![Postgres](https://github.com/GloriaY007/Final-Group-Project-/blob/Assitan_C/ScreenShots/Postgres.PNG?raw=true)

#### Connection String
We will use PSYCOPG2  as PostgresSQL adapter to test connectivity with Python. 

![Connection_string](https://github.com/GloriaY007/Final-Group-Project-/blob/Assitan_C/ScreenShots/Connection_string.PNG?raw=true)

### Database Interface
For our analysis, we will be using 3 different dataset from World Happiness, Freedom and Life Expectancy reports. The dataset will be loaded as csv files in Python. We will create 3 different dataframes : Happiness, Freedom and Life Expectancy, then merge them into one single dataframe. We will clean and preprocess the new dataframe then create our machine learning model for training.  

#### Mockup of machine learning

The team also collectively answered questions regarding the ***Presentation*** (see above). 

### Segment II: Build the Pieces

During the 2nd Segment, the project team, will be focused on building the separate pieces that compose the group project. During this phase, Gloria will be a :red_circle:, Lynn will be a :small_red_triangle:, Assitan will be a :heavy_multiplication_x:, and Diana will be a :black_square_button:.

Here is a list of deliverables for *Sunday, May 2, 2021* and their assigned reponsible team member:
- [x] Topic for the project 
- [x] Continuing with analysis and creating visuals to accompany the data story by @GloriaY007
     - [x] Presentation slides
     - [x] Description of the data exploration phase of the project
     - [x] Description of the analysis phase of the project
- [x] Refining of the machine learning model we'll be using (train and test) by @borkard
- [x] Outlining and beginning the work on a dashboard to house your final project. Checking and testing the work completed against the rubric by @assaci
- [x] Transforming of the mockup database into a full database that integrates with our work by @lynnokang

### Machine Learning Model Descriptions
#### Description of the preliminary data preprocessing
Prior to developing the machine learning model, the data from all three datasets (Happiness, Freedom, and Life-Expectancy) was cleaned by using Pandas to drop NaNs, duplicates, and unnecessary columns and the dataframes were merged to create one final dataframe. The datatypes of columns were also changed to be input in the machine learning model and the data was split by year into 2015 and 2016 dataframes. To pre-process the data for the machine learning model, Scikit-Learn was used to define the features and target sets and to scale the data with StandardScaler.

#### Description of preliminary feature engineering and preliminary feature selection
The target, y, is meant to be the output that the machine learning model will try to predict. For this project, happiness score was selected as the target and was created by using just that column from our final dataframe. The features for our machine learning model were selected by dropping the year and all columns from the happiness dataset and using all  the other columns as features, specifically from the Life Expectancy and freedom datasets. Some trial and error was done to select features with different levels of correlation with the target, but the best results came from using all columns other than those originally used to determine the happiness score in the happiness dataset.

#### Description of how data was split into training and testing sets
The data was split into training and testing sets by using the 2015 data as the training data and testing on the 2016 data. These dataframes were split by year from the original merged dataframe. This method produced a much higher accuracy score compared to using Scikit-Learn's train_test_split on the whole merged dataset.

#### Explanation of model choice, including limitations and benefits.
For our data, our group chose to use a supervised linear regression machine learning model to predict the happiness score of a country based on the features in the dataset. The benefits of using a linear regression model are that it will be able to predict the happiness score, a continuous variable,  based on the features of the data. A limitation of the linear regression model is that is assumes a linear relationship between the features and target and could miss some outliers or actual results that are not directly correlated.

### Dashboard

We will be using Tableau to create a storyboard of a dashboard to display data findings. For our analysis we are currently working with 3 different datasets from 2015 and 2016: World Happiness Report, Human Freedom Index, and Life expectancy Report. We've already merged the dataset into a dataframe in Pandas. The Dataframe was exported as a CSV file then loaded to Tableau Public. 

#### Storyboard

#### Happiness Score Per Country

Our merged dataset includes countries from 2015 and 2016. In addition, the countries are classified into regions. For our storyboard, we've already created an interactive world map that can be filtered on the country name, year, region, and happiness score. 

![Happiness_Map](https://github.com/GloriaY007/Final-Group-Project-/blob/Segment_2_Assitan_X/Happiness_Map.PNG?raw=true)


#### 10 happiest Countries and 10 least happiest countries 

We will create 2 charts to show the 10 happiest and least happiest countries for both 2015 and 2016. 

![Happiest](https://github.com/GloriaY007/Final-Group-Project-/blob/Segment_2_Assitan_X/Happiest.PNG?raw=true)


![Least_Happiest](https://github.com/GloriaY007/Final-Group-Project-/blob/Segment_2_Assitan_X/Least_Happiest.PNG?raw=true)

#### Correlation between data (still working on the chart)

We will create a chart to show the correlation between data and see which data has more impact on happiness score.
(Happiness score, economy_gdp_per_capita, family, health_life_expectancy,	freedom,	trust_government_corruption, generosity, pf_movement,	pf_religion,	pf_association,	pf_expression	pf_identity	pf_score,	ef_government,	ef_legal	and ef_money)

### Segment III: Plug It In

During the 3rd Segment, the project team, will be focused on pluging in the pieces we have put together. It involves wrapping up the analysis and content, and if needed, continuing to refine our code (including machine learning and database integration) and the images we'll include in our presentation for the group project. During this phase, Gloria will be a :small_red_triangle:, Lynn will be a :heavy_multiplication_x:, Assitan will be a :red_circle:, and Diana will be a :black_square_button:.

Here is a list of deliverables for *Sunday, May 9, 2021* and their assigned reponsible team member:
- [x] Continue to develop and refine the code for your analysis (Team) 
- [x] Create a draft presentation to share with your class by @GloriaY007
- [x] Complete peer reviews on the code by @borkard
- [x] Create a dashboard to display your findings by @assaci
- [x] Perform a quality assurance check on project deliverables against rubric requirements, and test the code by @lynnokang

## Draft Presentation



### Segment IV: Put It All Together

### Self-Assessment
