
# Richter's Predictor: Modeling Earthquake Damage
  01/2025-01/2025

**Team members**

- Group.

**Hosted by:** [DrivenData](https://www.drivendata.org/competitions/57/nepal-earthquake/)

## Overview

Based on aspects of building location and construction, your goal is to predict the level of damage to buildings caused by the 2015 Gorkha earthquake in Nepal.

![Nepal Earthquake Damage Map](https://s3.amazonaws.com/drivendata-public-assets/nepal-quake-bm-2.JPG)

This is an intermediate-level practice competition.  
The data was collected through surveys by **Kathmandu Living Labs** and the **Central Bureau of Statistics**, under the **National Planning Commission Secretariat of Nepal**. This survey is one of the largest post-disaster datasets ever collected, containing valuable information on earthquake impacts, household conditions, and socio-economic-demographic statistics.

---

## Problem Description

We're trying to predict the **ordinal variable** `damage_grade`, which represents a level of damage to the building that was hit by the earthquake. There are 3 grades:

- `1` → Low damage  
- `2` → Medium damage  
- `3` → Almost complete destruction  

![Screenshot](DamageGrade.png)


**Key Objectives:**
Task 1:-Prepare a complete data analysis report on the given data.

Task 2:-Create a predictive model in such a way that the objective is to predict the ordinal variable “damage_grade”. This column presents the level of damage grade affected by the earthquake.

Task 3:-Suggestions to the Seismologists to avoid earthquake event leading to significant damage in many buildings.

---

## Features

Each row in the dataset represents a specific building in the region affected by the Gorkha earthquake. The dataset has **39 columns**. The column `building_id` is a unique identifier. The remaining 38 features are described below:


---

## Results

Accuracy shows how often the model correctly predicts damage grades, giving a quick view of performance. However, with imbalanced classes, it can be misleading—so metrics like precision, recall, and F1-score are also important for a complete evaluation.

| Sl. No. | Regression Model      |    Train Accuracy (%) |   Test Accuracy (%) |
|:--------|:--------------------------|---------------:|--------------:|
|    1    | Logistic Regression        |       0.47|      0.41 |
|    2    | Logistic Regression tuned       |       0.57 |      0.48 |
|    3    | Random Forest|       0.98|      0.70|
|    4    | Random Forest tuned       |       0.73 |      0.70|
|    5    | Dicision tree        |       0.64|      0.98|
|    6    | XGBClassifire        |       0.80 |      0.70|
|    7    | XGBClassifire tuned             |       0.80 |      0.70|


## Seismologists to avoid earthquake event leading to significant damage in many buildings.

- Avoid construction on unstable land surfaces like 't'; enforce zoning regulations.
- Use stronger foundations, avoiding type 'r', and stabilize the ground.
- Improve roof ('n') and ground floor ('f') designs; avoid weak layouts like 'd'.
- Limit building heights or use seismic features like base isolators.
- Retrofit older and high-risk buildings with modern reinforcements.
- Design buildings for optimal family counts to avoid overloading.
- Use durable, flexible materials like reinforced concrete or steel.
- Train communities and builders on safe construction and preparedness.
- Integrate seismic data into urban planning for resilient cities.
- Implement seismic monitoring and early warning systems.

## Conclution
This project explores the complexities of earthquake damage prediction, aiming to classify damage grades using machine learning. By analyzing various factors such as building type, location, and structural integrity, we uncover valuable insights and select a robust model, Random Forest, for accurate damage grade classification.

Key Insights:
Various machine learning models were assessed, with the Random Forest model being chosen for earthquake damage prediction due to its robust performance.
The project used accuracy as the primary evaluation metric to assess model performance.
The Random Forest model achieved impressive results with 73% training accuracy and 70% testing accuracy, making it a suitable choice for predicting earthquake damage grades.
The insights from this project provide a comprehensive understanding of the factors influencing earthquake damage grades, derived from both exploratory data analysis and machine learning model perspectives. The Random Forest model's performance highlights its robustness and suitability for predicting damage grades based on various features. This project has not only enhanced our data science skills but has also deepened our understanding of earthquake damage prediction, marking a significant advancement in applying machine learning to disaster response and mitigation.

Thank you!!


