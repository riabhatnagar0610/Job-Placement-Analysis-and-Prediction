
# You're Hired!

This project performs job placement analyis and consists of machine learning models to predict which candidate will get hired based on certain criteria. 


## Roadmap

- Downloading the dataset and uploading it to Kaggle and Microsoft Excel

- Performing data cleaning and exploration

- Identifying trends and correlation between data features and target

- Building machine learning prediction models 


## Project Workflow

### Dataset

Context : Due to the growing need of educated and talented individuals, especially in developing countries, recruiting fresh graduates is a routine practice for organizations. Conventional recruiting methods and selection processes can be prone to errors and in order to optimize the whole process, some innovative methods are needed.

The dataset used can be found at the mentioned Kaggle link (https://www.kaggle.com/datasets/ahsan81/job-placement-dataset)

- This file contains different attribute of the candidates educational history and work experience. The detailed data dictionary is given below: 
  - gender : Gender of the candidate
  - ssc_percentage : Senior secondary exams percentage (10th Grade)
  - ssc_board : Board of education for ssc exams
  - hsc_percentage : Higher secondary exams percentage (12th Grade)
  - hsc_borad : Board of education for hsc exams
  - hsc_subject : Subject of study for hsc
  - degree_percentage : Percentage of marks in undergrad degree
  - undergrad_degree : Undergrad degree majors
  - work_experience : Past work experience
  - emp_test_percentage : Aptitude test percentage
  - specialization : Postgrad degree majors - (MBA specialization)
  - mba_percent : Percentage of marks in MBA degree
  - status (TARGET) : Status of placement. Placed / Not Placed


### Data Cleaning and Exploration 
Data cleaning is the process of ensuring data is correct, consistent and usable. You can clean data by identifying errors or corruptions, correcting or deleting them, or manually processing data as needed to prevent the same errors from occurring.

Data exploration is the first step of data analysis used to explore and visualize data to uncover insights from the start or identify areas or patterns to dig into more.

- explored the dataset for any duplicates and null values and corrected it where needed
- identifed patterns between different features of dataset and the result
- visualised the insights generated


### Trends and Patterns 
- If the candidate is placed or not on the basis of :
  - gender
  - specialization
  - work experience
  - hsc_subject and hsc_percentage
  - ssc_percentage

- number of males and females applied for the job
- from which specialization the candidates are placed in more number
- whether work experience is required to get placed
- which undergrad degree is best suited to get placed


### Machine Learning Models
First and foremost we'll import all the libraries needed for building the models:

// 

import numpy as np

import pandas as pd

import seaborn as sns

import matplotlib.pyplot as plt

from sklearn.model_selection import train_test_split

from sklearn.linear_model import LogisticRegression

from sklearn.metrics import accuracy_score,confusion_matrix

from sklearn.svm import SVC

from sklearn.naive_bayes import GaussianNB

from sklearn.neighbors import KNeighborsClassifier

from sklearn.tree import DecisionTreeClassifier

from sklearn.ensemble import RandomForestClassifier

from xgboost.sklearn import XGBClassifier

//

In the dataset we have a mix of categorical and numerical data. To build prediction models, we need to convert the categorical data into numerical.

For example, the below mentioned code converts the categorical data into binary:

//

data['gender'].value_counts()

gender_n = {'M':0,'F':1}

data['gender']=data['gender'].map(gender_n)

//

After conversion we'll build the prediction models using the following:
- Logistic Regression (accuracy - 0.8604651162790697)
- Guassian Naive Bayes (accuracy - 0.8604651162790697)
- K Neighbors Classifier (accuracy - 0.9069767441860465)
- Decision Tree Classifier (accuracy - 0.8604651162790697)
- Random Forest Classifier (accuracy - 0.9069767441860465)
- XGB Classifier (accuracy - 0.8837209302325582)


  
## Notes

If you find this insightful, feel free to star it. Any issues can be notified to me.

If you wanna work with this analysis, you can:

Clone the repository, or Fork the repository. Then, can make changes as you wish.
