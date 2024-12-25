# Project_Phase3

#### Project Overview

Access to clean and functional water sources is a fundamental necessity, yet many regions in Tanzania struggle to provide reliable water points for their population of over 67 million. Despite numerous water points being established across the country, a significant number are either non-functional or in need of repair. This situation hampers access to clean water, leading to health challenges, time lost in fetching water, and increased burdens on communities, particularly women and children.

This project seeks to address this issue by building a machine learning model to classify the operational status of water points. By analyzing data related to water point features such as pump type, installation details, and geographic characteristics, the project aims to predict whether a water point is functional, functional but requiring repair, or non-functional. Such insights can empower stakeholders to take targeted and proactive actions to improve water access.
#### Problem Statement
In Tanzania, many water points fail to provide reliable access to clean water, impacting millions of people and burdening rural communities. As a data scientist, my goal is to develop a machine learning model to predict the operational status of water points—functional, in need of repair, or non-functional. This will enable stakeholders to prioritize maintenance, allocate resources effectively, and address systemic issues, ensuring sustainable access to clean water for the population.
#### Data Understanding

Source: The dataset was sourced from Taarifa and the Tanzanian Ministry of Water and is available on DrivenData.
https://www.drivendata.org/competitions/7/pump-it-up-data-mining-the-water-table/page/23/

Features: The dataset includes attributes such as amount_tsh, funder, gps_height, installer, longitude, latitude, region, management, permit, construction_year, and more.

Target Variable: status_group (categorical: functional, functional needs repair, non-functional).
#### Data Preparation

Cleaning: Removed duplicate rows and handled missing values.

Feature Engineering: Dropped irrelevant columns (e.g., id, recorded_by) and applied one-hot encoding for categorical variables.

Scaling: Normalized numerical features using MinMaxScaler
#### Exploratory Data Analysis (EDA)

Visualized class distribution to address imbalance.

Analyzed feature importance to uncover key contributors to water point failures, such as construction_year, management
#### Modeling

Developed and evaluated three machine learning models:

Logistic Regression

Random Forest Classifier

Decision Tree Classifier

Performance Metrics: Accuracy, F1-Score, Precision, Recall, AUC-ROC.
#### Results and Insights

Best Model: Random Forest Classifier with a Macro-Averaged AUC of 0.63.

Key Insight:

Older water points and those managed by Village Water Committees (VWC) are more prone to failure.

#### Actionable Recommendations

Prioritize repairs for non-functional water points managed by VWC and WUG.

Build capacity for underperforming management groups and standardize practices across stakeholders.