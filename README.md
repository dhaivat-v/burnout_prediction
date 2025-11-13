🧠 Predicting Burnout Among Healthcare Workers During Crises

💡 Overview
This project uses data analytics and machine learning to predict burnout levels among healthcare workers during crisis periods (such as pandemics or emergencies).
The goal is to identify which factors — like workload, job satisfaction, and stress — most contribute to burnout, and to provide data-driven recommendations for prevention and support.

🧩 Objectives
-Analyse patterns of burnout in healthcare professionals across departments.

-Identify the strongest predictors of burnout.

-Use a Random Forest model to classify burnout levels as Never, Occasionally, or Often.

-Visualise how stress, job satisfaction, and workplace factors affect burnout.

-Offer actionable insights for hospital administrators and HR teams.

⚙️ Tools and Libraries

-Python 3.10+

-Pandas, NumPy – data handling and cleaning

-Matplotlib, Seaborn – visualisation

-Scikit-learn – machine learning (Random Forest, GridSearchCV)

📂 Dataset

-Dataset: Healthcare Workforce Mental Health Dataset
-Source: Kaggle – Healthcare Workforce Mental Health Dataset

Main Columns:

Column	Description
-Employee Type	Job title (e.g., Nurse, Technician, Administrator)
-Department (e.g., ICU, Paediatrics)
-Workplace Factor	: Main issue reported at work
-Stress Level	Rated 1–10
-Burnout Frequency	Target variable (Never, Occasionally, Often)
-Job Satisfaction	Rated 1–5
-Access to EAPs: Whether the worker has access to support programs
-Mental Health Absences: Number of mental-health-related absences
-Turnover Intention: Whether the worker intends to leave

🔬 Data Analysis Highlights
🔹 1. Feature Importance (Model Insight)

-Top predictors of burnout:

-Mental Health Absences 🧠

-Job Satisfaction 💼

-Stress Level ⚡

🔹 2. Burnout by Department

-Highest burnout levels in General Medicine and ICU.

-Administrative roles show the lowest burnout rates.

🔹 3. Burnout by Workplace Factor

-Heavy workload and poor work environment are the biggest contributors.

🔹 4. Correlation Findings

-Higher stress → more mental health absences (+0.50 correlation).

-Higher stress → lower job satisfaction (–0.38 correlation).

🧮 Model Performance

Metric	Baseline	Tuned Model
Accuracy	0.52	0.56
F1 (Often Burnout)	0.62	0.69
Recall (Often Burnout)	0.67	0.78

Best Parameters:
{'max_depth': 10, 'min_samples_leaf': 1, 'min_samples_split': 2, 'n_estimators': 300}

The tuned Random Forest model performs best at identifying healthcare workers who experience frequent burnout — the most critical group for intervention.

📈 Key Visual Insights

-ICU and General Medicine show the highest average stress levels.

-Heavy Workload overwhelmingly drives burnout.

-Strong negative correlation between stress and job satisfaction.

(See figures in the notebook under “Visualization Results.”)

💭 Conclusion and Recommendations

-Mental health absences, job satisfaction, and stress are the leading indicators of burnout.

-Hospitals should monitor these metrics regularly to detect early burnout risk.

-Implementing better workload balance and enhancing Employee Assistance Programs (EAPs) could significantly reduce burnout levels.

-Data-driven wellness policies can improve staff retention and patient care quality.

🧰 Repository Structure
burnout_prediction/
│
├── data/
│   └── Healthcare_Workforce_Mental_Health_Dataset.csv
├── notebooks/
│   └── burnout_prediction.ipynb
├── outputs/
│   └── burnout_visuals.png
├── README.md
└── requirements.txt

✨ Author
Dhaivat Vyas
🎓 Bachelor of Health Science (Public Health & Health Promotion) – Deakin University
📊 Google Data Analytics Certified | IBM Data Science Learner | Deloitte Job Simulation Certified
📍 Based in Australia
