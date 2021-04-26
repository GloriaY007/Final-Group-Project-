# Final-Group-Project
Shared repository for final group project

## Presentation

#### Selected topic
The team would like to explore the topic of *Happiness and its contributing factors*

#### Reason they selected the topic 
The team selected this topic because we were trying to find what defined happiness. We were also looking for a good and clean dataset with solid features and information to train a machine on.

#### Description of the source of data
The main dataset being used is a collection of data from the [World Happiness Report](https://www.kaggle.com/unsdsn/world-happiness). It is a landmark survey of the state of global happiness. The data set has a collection of indicators on more than **140 countries** around the world including happiness rank, happiness score on a scale of 0 to 10, standard error, and more… The data set includes reports from 2015 to 2019. 

We will also be using the [World Bank Life Expectancy](https://data.worldbank.org/indicator/SP.DYN.LE00.IN) data set and the [Human Freedom Index](https://www.kaggle.com/gsutters/the-human-freedom-index), to compare against (for the years that align with our main data set). 

#### Questions they hope to answer with the data
We want to find which factors influence happiness within a country and we would also like to found. out how to predict the happiness scores, if it is at all possible to do so.

## Communication Plan

The communication plan will be a guiding document outlining our means of communication, and our risk and issues management. It also outlines the team structure, the roles and responsibilities of each team member per segment, and our approval process for our work.

### Communications Tools for "The Ladies" a.k.a Group 2 project team

#### Team Structure

The team structure is modeled around **four (4) roles**. The roles will be rotated troughout the lenght of the project amongst the four (4) students composing the team. The roles are structured as explained below:
- **Square**: The team member in the square role will be responsible for the repository.
- **Triangle**: The member in the triangle role will create a mockup of a machine learning model. This can even be a diagram that explains how it will work concurrently with the rest of the project steps.
- **Circle**: The member in the circle role will create a mockup of a database with a set of sample data, or even fabricated data. This will ensure the database will work seamlessly with the rest of the project.
- **X**: The member in the X role will decide which technologies will be used for each step of the project

The members composing this team are:
- Assitan Cissé
- Dian Borkar
- Merelynn (Lynn) Okang
- Gloria Yahouedeou

#### Meeting Plan

In addition to actively using the designated Slack channel created for Group 2 for chats and questions, the team has agreed to three weekly timeslots to collaborate on the project:
- Mondays from 6-8 pm EST.
- Fridays from 6-8 pm EST. (During Office Hours)
- Sundays from 7-11 pm EST. (Work submission review)

Team members unable to attend these group work opportunities use the Slack channel to notify other members of progress, issues, or availability.

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


#### Risk and Issue Management

This team recognize that risk and issue may arise trough the course of our collaboration. The team has listed below potential problems that might arise during the project, their causes, symptoms, consequences, and possible solutions.

| Date Recorded | Risk Description | Probability | Impact | Mitigation Plan |
| ------------- | ------------- | ------------- | ------------- | ------------- |
| 22 Apr 21  | Choosing a database that provides a poor machine learning output  | Medium | High  | Consulting TAs to guide us at each step of the process |
| 22 Apr 21  | A team member feeling overworked or underworked  | Medium  | Medium  | For each segment, the team agrees to a breakdown of the deliverables and offer/receives support where needed   |
     

The risk register above will be periodically updated to list any issue that may have come up. For high propability and high impact issue that have no mitigation in place, the team will:

![Risk Escalation Process](https://github.com/GloriaY007/Final-Group-Project-/blob/GloriaY-S/Risk%20Ecalation%20Process.png)

### Segment I: Sketch It Out!

During the 1st Segment,  ***The Ladies*** project team, will be focused on outlining the structure of the overall group project. During this phase, Gloria will be a square, Lynn will be a triangle, Assitan will be a circle, and Diana will be an X.

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

#### Mockup of machine learning


The team also collectively answered questions regarding the ***Presentation*** (see above). 

### Segment II: Build the Pieces

### Segment III: Plug It In

### Segment IV: Put It All Together

### Self-Assessment

