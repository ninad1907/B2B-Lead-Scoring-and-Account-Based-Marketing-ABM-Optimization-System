# B2B-Lead-Scoring-and-Account-Based-Marketing-ABM-Optimization-System

 Project Overview
X Education, an online course provider for industry professionals, generates a large number of leads daily but struggles with a low conversion rate (~30%). The goal of this project is to develop a Lead Scoring Model using Logistic Regression to predict the likelihood of lead conversion. The model assigns a lead score (0-100) to prioritize high-potential leads and improve conversion rates to the CEO's target of 80%.

📊 Dataset Overview
The dataset consists of 9,240 rows and 37 columns, containing information about lead interactions, demographics, and engagement levels.

Key Features:
Lead Source: The platform where the lead was generated (e.g., Google, Facebook, Direct Traffic, etc.)
Lead Origin: How the lead first interacted (e.g., API, Landing Page Submission)
Total Time Spent on Website: Time spent by the lead on the website (numerical)
Page Views Per Visit: Number of pages viewed per session
Last Activity: The most recent action taken by the lead (e.g., Email Opened, SMS Sent)
Specialization: The professional field of the lead (e.g., IT, Marketing, Finance)
Converted (Target Variable): 1 if the lead converted, 0 otherwise
🔍 Data Preprocessing
1. Handling Missing Values
Columns with >40% missing values were dropped (e.g., 'City').
Categorical missing values were filled using mode (most frequent value).
Rows with <2% missing values were dropped to maintain data integrity.
2. Feature Engineering & Encoding
Categorical variables were encoded using one-hot encoding.
Numerical variables were scaled using StandardScaler.
Irrelevant columns (e.g., 'Lead Number') were dropped.
📈 Model Development
Logistic Regression for Lead Scoring
Train-Test Split: 70% training, 30% testing
Feature Selection: Used Recursive Feature Elimination (RFE)
Performance Metrics:
Accuracy
Precision & Recall (to handle class imbalance)
ROC-AUC Score (to evaluate model discrimination ability)
📊 Model Evaluation & Results
Final Accuracy: 91.26% ✅
Precision: 95.96% 🎯 (High precision means fewer false positives)
Recall: 83.01% 🔄 (Ensures most potential leads are captured)
ROC-AUC Score: 94.94% 📈 (Indicates strong model performance)
The model successfully improved the lead prioritization, enabling the sales team to focus on high-converting leads and increase efficiency.
📌 Business Impact
✅ Increased Lead Conversion Rate: More focused sales efforts led to higher conversion rates. ✅ Optimized Marketing Strategies: Identified the best lead sources for high conversions. ✅ Reduced Resource Wastage: Sales team spent less time on low-potential leads.

🛠 Technologies Used
Python (Pandas, NumPy, Scikit-Learn, Seaborn, Matplotlib)
Machine Learning (Logistic Regression, Feature Engineering, Model Evaluation)
Jupyter Notebook for Analysis & Visualization
