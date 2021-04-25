# Final-Group-Project-

## Database Storage Set Up 
PostgreSQL will be used for database storage. 
- Happiness RDS instance was already set up in ASW.The database was made public so everyone can have access.
- A new server happiness and a database Final_ Project were created on PostgreSQL. 
![AWS](https://github.com/GloriaY007/Final-Group-Project-/blob/Assitan_C/ScreenShots/AWS.PNG?raw=true)

![Postgres](https://github.com/GloriaY007/Final-Group-Project-/blob/Assitan_C/ScreenShots/Postgres.PNG?raw=true)

## Connection String
We will use PSYCOPG2  as PostgresSQL adapter to test connectivity with Python. 
![Connection_string](https://github.com/GloriaY007/Final-Group-Project-/blob/Assitan_C/ScreenShots/Connection_string.PNG?raw=true)

## ERD
![ERD](https://github.com/GloriaY007/Final-Group-Project-/blob/Assitan_C/ScreenShots/ERD.png?raw=true)

## Database Interface
For our analysis, we will be using 3 different dataset from Worl Happiness, Freedom and Life Expectancy reports. The dataset will be loaded as csv files in Python. We will create 3 different dataframes : Happiness, Freedom and Life Expectancy, then merge them into one single dataframe. We will clean and preprocess the new dataframe then create our machine learning model for training.  








