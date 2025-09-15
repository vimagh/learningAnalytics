---Data-Driven Decision-Making and Performance Enhancement in Educational Institutions
--Project Overview
This project leverages the Open University Learning Analytics Dataset (OULAD) to predict student performance outcomes and enable proactive educational interventions. By integrating machine learning models with a Power BI Learning Analytics Dashboard, the study demonstrates how data-driven tools can identify at-risk students, monitor engagement, and provide actionable insights for educators and policymakers.

Motivation
Educational institutions in developing countries face systemic challenges such as limited resources, lack of data-driven tools, and high dropout rates. This project was motivated by the need to:
Improve student retention and success rates.


Provide educators with interpretable insights for intervention.


Showcase how learning analytics dashboards can transform decision-making in higher education .



Code and Resources Used
Programming Languages: Python (pandas, scikit-learn, matplotlib, seaborn)


Visualization: Power BI


Dataset: Open University Learning Analytics Dataset (OULAD)


Machine Learning Models: Logistic Regression, Decision Tree, Random Forest, Gradient Boosting



Data Collection
The dataset was sourced from the Open University (UK) and hosted publicly on Kaggle. It contains seven tables including:
StudentInfo (demographics, age, gender, prior education)


StudentAssessment & Assessment (submission dates, scores, weights)


StudentVLE & VLE (Virtual Learning Environment interactions, clicks, activity types)


StudentRegistration (enrollment and withdrawal data) .



EDA
Exploratory Data Analysis (EDA) revealed:
Assessment submission and high scores are the strongest predictors of success.


Older and more educated students perform better.


Students with disabilities face higher risk of withdrawal and failure.


Engagement (VLE clicks) strongly correlates with pass rates .



Preprocessing and Feature Engineering
Merged 7 raw tables into a unified dataset.


Missing values imputed or dropped (sparse fields like date_unregistration).


Categorical encoding for demographics and education.


Standardization applied to numerical features.


Selected features: Age, Gender, Disability status, Module attempts, Assessment submission, Previous education, Final score .



Model Performance
Several classification models were trained and evaluated:The Random Forest Classifier showed the best balance, particularly excelling at recall (correctly identifying at-risk students) .

Model Explainability
Feature importance (Random Forest):


Assessment submission


Module attempts


Disability status


Previous education


VLE engagement


Explainability ensured the model’s predictions were transparent and actionable for educators .



Productionization
The final Random Forest model was integrated into a Power BI Dashboard that provides:
KPI Panels: Retention, engagement, at-risk students, average CGPA


Demographics View: Age, disability status, education, gender


Assessment Adherence Tracker: Monitors submission trends


Engagement Monitor: Tracks VLE interactions


This allows real-time, interpretable insights for non-technical stakeholders .
