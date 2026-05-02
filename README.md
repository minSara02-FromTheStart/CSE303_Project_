# CSE303_Project_

This project analyzes the Student Performance Factors dataset to identify key variables that influence students' academic performance. The analysis combines statistical exploration, visualization, and machine learning (Linear Regression) to derive meaningful insights.

Number of observations (rows): 6607
Number of features (columns): 20

🔢 Numerical Features
1.Hours_Studied
2.Attendance
3.Sleep_Hours
4.Previous_Scores
5.Tutoring_Sessions
6.Physical_Activity
7.Exam_Score

🔠 Categorical Features
1.Parental_Involvement
2.Access_to_Resources
3.Motivation_Level
4.Family_Income
5.Teacher_Quality
6.School_Type
7.Peer_Influence
8.Gender
9.Internet_Access
10.Extracurricular_Activities
11.Learning_Disabilities
12.Parental_Education_Level
13.Distance_from_Home

📊 Project Workflow

1️⃣ Exploratory Data Analysis (EDA)
Central tendency (mean, median, mode)
Dispersion (variance, standard deviation, IQR)
Distribution analysis using histograms & boxplots
Correlation analysis using heatmap

2️⃣ Categorical Analysis
Frequency distribution of key variables
Identification of imbalance (e.g., Internet Access ~92%)

3️⃣ Relationship Analysis
Strong positive correlation:
Attendance → Exam Score
Moderate relationship:
Hours Studied → Exam Score
Weak relationship:
Previous Scores → Exam Score

🧹 Data Preprocessing

Missing values handled using mode imputation
No duplicate records found
Outlier detection using IQR method

👩‍🚒 Feature engineering:

study_efficiency = Previous_Scores / (Hours_Studied + 1)
engagement = Attendance × Hours_Studied

🤖 Machine Learning Model

Model Used:
Linear Regression
Techniques Applied:
Normal Equation (Manual Implementation)
Gradient Descent (α = 0.01, iterations = 1000)
Scikit-learn LinearRegression
Train-Test Split:
70% Training / 30% Testing

📈 Model Performance

| Model                     | RMSE     |
| ------------------------- | -------- |
| Normal Equation           | 2.28     |
| Sklearn Model             | 2.28     |
| Gradient Descent          | 2.29     |
| With Categorical Features | **1.86** |

➡️ Adding categorical features improved performance by ~18%

🔍 Key Insights

📌 Attendance is the most important factor affecting exam scores
📌 Most students have moderate study habits (normal distribution)
📌 Parental involvement strongly influences top performers
📌 The top 3 predictors:
Attendance
Study Hours
Parental Involvement

📊 Visualizations

Histograms & Boxplots
Correlation Heatmap
Actual vs Predicted Graph
Gradient Descent Convergence Plot

🧠 Conclusion

This project demonstrates how combining EDA + Feature Engineering + Regression Modeling can effectively predict student performance and uncover real-world educational insights.

🚀 Future Improvements

Try advanced models (Random Forest, XGBoost)
Perform hyperparameter tuning
Deploy as a web app (Streamlit)
Add real-time prediction interface
