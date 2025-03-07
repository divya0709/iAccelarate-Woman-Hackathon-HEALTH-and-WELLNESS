iAccelerate Women's Hackathon - HEALTH & WELLNESS

Menstrual Cycle Data Analysis

This repository contains the code for analyzing the Menstrual Cycle Data and segmenting women's health profiles using Hierarchical Clustering and Gaussian Mixture Models (GMM). 
The objective is to provide personalized healthcare recommendations based on menstrual health data.

📊 Dataset Information
Source: Menstrual Cycle Data
Author: Richard J. Fehring, Marquette University
Publication Date: 2012
Data Usage: This dataset has been anonymized for dissemination. Data reuse was agreed to by subjects in the consent form.
Features: 80 attributes related to menstrual health, such as cycle length, bleeding intensity, age, BMI, etc.
Rows: 1665
⚠️ Note: Due to licensing restrictions, the dataset is NOT included in this repository. You can download it from [Menstrual Cycle Data](https://epublications.marquette.edu/data_nfp/7)


🔍 Problem Statement
Women have diverse health needs that are often not adequately addressed by generic healthcare approaches.
This lack of personalization can lead to suboptimal health outcomes and limited access to relevant services.

Objective
Develop a data-driven solution using Hierarchical Clustering and Gaussian Mixture Models (GMM) to segment women based on their health needs and preferences. 
The goal is to create personalized healthcare recommendations that enhance access to services and improve health outcomes.

🏗 Methodology
Data Preprocessing
Dropped irrelevant columns (e.g., 'Group', 'CycleNumber').
Handled missing values (median for numerical, mode for categorical).
Created binary features for missing values in critical columns.
Standardized the data for better clustering performance.
Clustering Techniques Used
1️⃣ Hierarchical Clustering
Used single linkage clustering to segment women based on health-related features.
Identified 3 clusters using a dendrogram.
📊 Visualization: Dendrogram showing hierarchical clustering structure.
2️⃣ Gaussian Mixture Model (GMM)

Determined the optimal number of clusters using the Silhouette Score.
Identified 3 optimal clusters.
📊 Visualization: Silhouette Score plot.
📌 Cluster Analysis & Insights
| Cluster | Characteristics                          | Insights                                                  |
|---------|-----------------------------------------|----------------------------------------------------------|
| Cluster 1 | Regular Cycle with High Fertility      | Ideal for optimizing conception and reproductive health maintenance. |
| Cluster 2 | Irregular Cycles with Anovulation     | Requires ovulation tracking and lifestyle changes. |
| Cluster 3 | Postpartum or Breastfeeding           | Focus on postpartum recovery, fertility awareness, and nutritional support. |
| Cluster 4 | Menstrual Disorders (PCOS, Endometriosis) | Needs symptom management and possible medical intervention. |
| Cluster 5 | Perimenopausal or Menopausal          | Focus on managing hormonal changes and long-term health. |
| Cluster 6 | General Menstrual Health              | General advice on maintaining menstrual health and lifestyle. |



📂 Files in This Repository
README.md → Project documentation
menstrual_data_analysis.ipynb → Jupyter Notebook with clustering analysis

Clone the repository:
bash
git clone https://github.com/divya0709/iAccelarate-Woman-Hackathon-HEALTH-and-WELLNESS.git
cd iAccelarate-Woman-Hackathon-HEALTH-and-WELLNESS
Open the Jupyter Notebook and run the analysis:
  jupyter notebook menstrual_data_analysis.ipynb

📌 Future Scope
Enhance the dataset with more diverse health parameters.
Deploy the clustering model into a healthcare app for real-world application.
Integrate AI-driven insights for personalized health tracking and recommendations.
📌 Python Notebook: [Kaggle Notebook](https://www.kaggle.com/code/divyapancholi/menstrual-dataset)

