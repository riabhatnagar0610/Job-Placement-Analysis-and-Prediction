# You're Hired!

This project aims to analyze candidate data and build machine learning models to predict whether a candidate will be hired or not. The project focuses on leveraging various features from candidate profiles, such as education, experience, skills, etc., to predict job placement outcomes accurately.

## Table of Contents
- [Introduction](#introduction)
- [Installation](#installation)
- [Data](#data)
- [Features](#features)
- [Modeling](#modeling)
- [Evaluation](#evaluation)
- [Contributing](#contributing)


## Introduction
In today's competitive job market, it is crucial for both candidates and recruiters to make informed decisions. This project offers an automated solution to predict job placement outcomes based on candidate data. By analyzing various features, the machine learning models aim to provide insights into a candidate's likelihood of being hired.

## Installation
To use this project, you need to have Python 3.x installed on your system. Clone the repository and install the required dependencies using the following command:

pip install -r requirements.txt

## Data
The dataset used in this project consists of candidate profiles with various attributes, such as education, experience, skills, and more. It is important to ensure that the dataset is properly prepared and formatted before running the project. The `Job_Placement_Data.csv` file contains the dataset used for analysis and prediction. 

## Features
The candidate features considered in this project include:
- Education: Candidate's educational background (e.g., degree, field of study, board percentage).
- Experience: Candidate's previous work experience (e.g., number of years).
- Specialisation: Candidate's skills and qualifications relevant to the job.
- Industry: The industry in which the candidate is seeking a job placement.
- Gender: It plays an important role in finding out the ratio of women to men and if there exists any bias.

## Modeling
The project utilizes various machine learning algorithms to predict job placement outcomes. Some of the models employed are:
- Logistic Regression
- Random Forest
- Support Vector Machine (SVM)
- Gradient Boosting

These models are trained on the provided dataset to learn patterns and make accurate predictions.

## Evaluation
To evaluate the performance of the machine learning models, the project utilizes various metrics such as accuracy, precision, recall, and F1 score. These metrics provide insights into the model's ability to correctly predict job placement outcomes.
The highest accuracy acheived is 91% from Random Forest Classifier and K Neighbors classifier.

## Contributing
Contributions to this project are welcome. If you find any issues or have suggestions for improvements, please open an issue or submit a pull request.
