# Predicting Response Time of Paris Fire Brigade Vehicles

The Challenge is taken from https://paris-fire-brigade.github.io/data-challenge/challenge.html

## Problem Statement
The response time is one of the most important factors for emergency services because their ability to save lives and rescue people depends on it. A non-optimal choice of an emergency vehicle for a rescue request may lengthen the arrival time of the rescuers and impact the future of the victim. This choice is therefore highly critical for emergency services and directly relies on their ability to predict precisely the arrival time of the different units available.

## Overview
This project aims to predict the response time of the Paris Fire Brigade vehicles. The prediction focuses on the delay between the selection of a rescue vehicle and its arrival at the scene of the rescue request.

## Project Members
- Yashas J (USN: 01FE17BCS244)
- Akash B (USN: 01FE17BCS020)
- Akhila A. G (USN: 01FE17BCS022)
- Aishwarya G. M (USN: 01FE17BCS016)

## Academic Year
2019-2020

## Institution
KLE Technological University, Hubli

## Guide
Prof. Neha T

## Abstract
The project uses data mining techniques to predict the response times of Paris Fire Brigade vehicles. The predictions are based on the previous year's data (2018), and the project employs methods such as Ridge, Lasso, and Linear Regression.

## Objectives
1. Develop models to predict the delay between the selection of a rescue vehicle and its arrival at the scene.
2. Apply data mining techniques to approach the problem.
3. Select relevant attributes using appropriate techniques.
4. Compare the performance of different classification techniques.

## Data Description
- **Training Data**: 
  - Size: 200 MB
  - Attributes: 26
  - Tuples: 219,338
- **Test Data**: 
  - Size: 98.2 MB
  - Attributes: 26
  - Tuples: 108,034

### Key Attributes
- Emergency vehicle selection
- Alert reason category
- Location of the event
- Longitude and latitude of intervention
- Emergency vehicle type
- Rescue centre
- Selection date and time
- OSRM estimated distance and duration

## Methodology
1. **Data Preprocessing**
   - Remove IDs
   - Fill NULL values
   - Handle outliers
   - Convert categorical data to numerical data
2. **Modeling**
   - Apply Linear Regression, Lasso Regression, Ridge Regression, and Light GBM
3. **Evaluation**
   - Use metrics such as R² score to evaluate model performance
   - Employ k-Fold Cross-Validation

## Results
- **Linear Regression**
  - R² score for train data: 0.166
  - R² score for test data: 0.125
- **Lasso Regression**
  - R² score for train data: 0.15
  - R² score for test data: 0.105
- **Ridge Regression**
  - R² score for train data: 0.1482
  - R² score for test data: 0.125
- **Light GBM**
  - R² score for train data: 0.292
  - R² score for test data: 0.1806

## Conclusion
The models developed provide a framework for predicting the response times of emergency vehicles. The use of different regression techniques helps in understanding their effectiveness and limitations in predicting such events.

## Acknowledgements
We thank Prof. Neha T for her guidance and support. We also thank Prof. Shankar S and Prof. P. G. Sunitha Hiremath for their assistance. Special thanks to Dr. Meena S M, Head of the Department, for providing the necessary academic environment.

## References
- https://paris-fire-brigade.github.io/data-challenge/challenge.html
- https://challengedata.ens.fr/participants/challenges/21/
- https://medium.com/crim/predicting-the-response-times-of-firefighters-using-data-science-da79f6965f93
- https://eng.uber.com/engineering-an-efficient-route/
- https://pandas.pydata.org/pandas-docs/stable/reference/api/pandas.get_dummies.html
- https://www.youtube.com/watch?v=9yl6-HEY7_s
- http://www.datasciencemadesimple.com/convert-column-to-categorical-pandas-python-2/
