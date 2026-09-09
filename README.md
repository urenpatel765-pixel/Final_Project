# 🎓 Smart Outcome Predictor

### Ensemble Learning-Based Student Outcome Prediction

> A comprehensive Machine Learning project for predicting student course completion and final academic performance using Bagging, Boosting, Voting and Stacking Ensemble techniques.

---

## 📌 Project Overview

**Smart Outcome Predictor** is an academic Machine Learning project that investigates how Ensemble Learning techniques can be applied to educational data to predict student outcomes.

The project addresses two supervised learning problems:

1. **Classification** — predicting whether a student completes a course.
2. **Regression** — predicting the student's final academic score.

The study compares a single Decision Tree baseline with several ensemble approaches, including:

- Bagging
- AdaBoost
- Gradient Boosting
- LightGBM
- XGBoost
- Hard Voting
- Soft Voting
- Stacking

The project goes beyond simply training models. It also evaluates:

- Data quality
- Feature engineering
- Missing-value handling
- Leakage prevention
- Cross-validation
- Hyperparameter behaviour
- Generalisation
- Overfitting
- Feature importance
- Robustness
- Computational efficiency
- Business interpretation

The final experiments show that ensemble learning can substantially improve upon the single Decision Tree baseline, although the best model depends on the evaluation objective.

---

## 🎯 Problem Statement

Educational platforms generate valuable information about how students interact with courses.

Examples include:

- Learning sessions
- Time spent studying
- Videos watched
- Quiz attempts
- Assignment submissions
- Forum participation
- Quiz performance
- Attendance

The objective of this project is to determine whether these variables can be used to build reliable predictive models for student outcomes.

The project therefore asks:

> **Can Ensemble Learning methods effectively predict student course completion and final academic performance from demographic, course, behavioural, engagement and attendance-related features?**

---

## 💡 Motivation

Early identification of students who may struggle with course completion or academic performance can potentially help educational institutions provide timely support.

A predictive system could support activities such as:

- Early academic intervention
- Student counselling
- Learning support
- Engagement monitoring
- Academic planning
- Personalised assistance

However, predictions should be treated as **decision-support information**, not as automatic academic decisions.

The purpose of this project is therefore to investigate the predictive capability of Ensemble Learning methods while also examining their limitations and generalisation behaviour.

---

# 🎯 Project Objectives

The major objectives are:

### Data Understanding
- Understand the dataset structure and variables.
- Identify numerical and categorical features.
- Analyse missing values and duplicates.
- Study the classification and regression targets.

### Data Preparation
- Remove identifier-only information.
- Engineer useful date features.
- Handle missing values.
- Encode categorical variables.
- Scale numerical variables.
- Prevent target leakage.

### Model Development
Implement and compare:

- Decision Tree
- Bagging
- AdaBoost
- Gradient Boosting
- LightGBM
- XGBoost
- Hard Voting
- Soft Voting
- Stacking

### Model Evaluation
Use appropriate metrics for both tasks.

**Classification:**
- Accuracy
- Precision
- Recall
- F1-score
- ROC-AUC

**Regression:**
- MAE
- RMSE
- R²

### Advanced Analysis
- 5-fold cross-validation
- Hyperparameter analysis
- Robustness testing
- Feature importance
- Generalisation analysis
- Training-time comparison
- Practical interpretation

---

# 🔬 Research Questions

The project investigates the following questions:

1. Can ensemble methods outperform a single Decision Tree?
2. How effective is Bagging compared with a single tree?
3. How do AdaBoost, Gradient Boosting, LightGBM and XGBoost compare?
4. Does Voting improve classification performance?
5. Does Stacking provide additional predictive improvement?
6. Which model performs best for course-completion classification?
7. Which model performs best for final-score regression?
8. Which student features contribute most strongly to model predictions?
9. How well do the models generalise to unseen data?
10. Does greater model complexity necessarily produce better results?

---

# 📊 Dataset

The project uses a student learning dataset containing **5,200 records and 19 original columns**.

### Dataset Summary

| Property | Value |
|---|---:|
| Records | 5,200 |
| Original Columns | 19 |
| Duplicate Rows | 0 |
| Processed Features | 34 |
| Classification Target | `completion_status` |
| Regression Target | `final_score` |
| Train-Test Split | 80% / 20% |
| Cross-Validation | 5-Fold |
| Random State | 42 |

---

# 📋 Dataset Features

| Feature | Type | Description |
|---|---|---|
| `student_id` | ID | Student identifier |
| `age` | Numerical | Student age |
| `country_region` | Categorical | Geographic region |
| `device_type` | Categorical | Learning device |
| `education_background` | Categorical | Educational background |
| `course_level` | Categorical | Course level |
| `course_category` | Categorical | Course category |
| `course_start_date` | Date | Course start date |
| `week_of_year` | Numerical | Course start week |
| `sessions` | Numerical | Learning sessions |
| `time_spent_hours` | Numerical | Learning time |
| `videos_watched` | Numerical | Videos watched |
| `quiz_attempts` | Numerical | Quiz attempts |
| `assignments_submitted` | Numerical | Assignments submitted |
| `forum_posts` | Numerical | Forum participation |
| `avg_quiz_score` | Numerical | Average quiz score |
| `attendance_rate` | Numerical | Attendance rate |
| `completion_status` | Target | Course completion |
| `final_score` | Target | Final academic score |

---

# 🧹 Data Quality Analysis

The dataset was inspected before model training.

The analysis included:

- Dataset dimensions
- Data types
- Missing values
- Duplicate records
- Target distribution
- Numerical statistics
- Categorical variables

### Duplicate Records

No duplicate rows were identified.

```text
Duplicate Rows = 0
