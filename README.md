# Phase-3-Project
### 🧬 Flu Vaccine Prediction Project
This project explores the factors influencing vaccine uptake during the H1N1 and seasonal influenza outbreaks using machine learning models. It aims to predict individuals' likelihood to take either vaccine and uncover key features contributing to vaccine hesitancy.

#### 📌 Project Overview
Vaccine hesitancy presents a significant public health challenge, especially during pandemics. By analyzing demographic, behavioral, and opinion-based data, this project builds predictive models to identify patterns and drivers of vaccine uptake. Insights gained here can help design better-targeted awareness campaigns and health interventions.

#### 🧠 Business and Data Understanding
##### Business Objective:
To assist public health agencies in improving vaccination rates by identifying key hesitancy drivers and predicting individuals less likely to get vaccinated for H1N1 and seasonal influenza.

##### Data Source:
Data was obtained from the DrivenData "Flu Shot Learning" competition. It contains:

Demographics (age, race, education, income)

Behavior and risk perception (mask usage, gathering behavior, health worker status)

Opinions on vaccine effectiveness and safety

Labels indicating whether the individual received H1N1 and/or seasonal flu vaccines.

#### 🧮 Problem Statement
To develop predictive models that:

~ Classify individuals based on their likelihood of receiving H1N1 and/or seasonal influenza vaccines.

~ Identify the most influential factors contributing to vaccine hesitancy.

#### 🎯 Objectives
1. Predict H1N1 and seasonal flu vaccine uptake using machine learning.

2. Compare performance of different models (e.g., Logistic Regression, Decision Tree).

3. Evaluate model performance using AUC scores.

4. Identify and rank key predictive features.

5. Provide recommendations for improving vaccine campaigns based on insights.

##### 🧹 Data Preprocessing
Missing values were imputed using appropriate strategies, mode for the categorical data and mean for numerical data.

Categorical variables were encoded using one-hot encoding.

Feature scaling was done using StandardScaler to normalize input for models.

The dataset was split into training and testing sets (80/20 split).

##### 🧪 Modeling
Two models were trained separately for each target (H1N1 and Seasonal vaccines):

Logistic Regression: For interpretability and baseline comparison.

Decision Tree Classifier: To visualize decision paths and extract rules.

Each model was trained, and class probabilities were predicted. ROC-AUC scores were used for evaluation.

##### 📊 Evaluation
Model	H1N1 AUC	Seasonal AUC	Mean AUC
Logistic Regression	0.826	0.852	0.839
Decision Tree	0.818	0.828	0.823

Logistic Regression outperformed Decision Trees in both categories, making it the preferred model for deployment.

##### 🔍 Feature Importance
##### From Logistic Regression:

###### Top predictors for H1N1 uptake:

~ Doctor recommendation

~ Belief in H1N1 vaccine effectiveness

~ Perceived risk of H1N1

~ Health worker status

###### Top predictors for Seasonal uptake:

~ Perceived seasonal flu risk

~ Doctor recommendation

~ Belief in seasonal vaccine effectiveness

~ Age group (65+)

#### ✅ Conclusion
Machine learning models successfully predicted vaccine uptake with strong performance. Logistic Regression provided both high accuracy and explainability. The most influential features suggest that trust in healthcare providers and perceived risk significantly drive vaccination behavior.

#### 💡 Recommendations
~ Targeted Campaigns: Focus on populations with lower trust in vaccines and healthcare providers.

~ Healthcare Provider Involvement: Leverage doctor recommendations as a powerful motivator.

~ Educational Outreach: Combat misconceptions about vaccine safety, especially for seasonal flu.

~ Age-Based Messaging: Customize messaging for different age demographics.

#### 🚀 Deployment Potential
This model can be integrated into public health systems to:

1. Predict which communities or individuals are less likely to vaccinate.

2. Prioritize outreach resources.

3. Simulate impact of various messaging strategies using key features.

##### 📂 Project Structure
Business Understanding
Data Understanding
Data Preparation
Modeling
Evaluation
Code Quality

##### 📦 Requirements
Main libraries:
pandas
numpy
scikit-learn
matplotlib
seaborn


🙋‍♀️ Author
Doreen Murugi
Data Science Bootcamp Student @ Moringa School


