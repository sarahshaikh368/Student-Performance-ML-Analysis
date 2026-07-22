# Student Performance Analysis & Machine Learning Investigation

## Project Overview
This project analyzes student academic performance using tabular data, performs Exploratory Data Analysis (EDA), builds baseline and advanced Machine Learning models, and evaluates their predictive accuracy.

## Dataset Overview
* **Dataset Name:** Student Performance Dataset (`student.csv`)
* **Total Records:** 30
* **Features:** 9 features (AGE, ATTENDANCE, VIDEO GAMES, TUITION, HEALTH, STRESS, DAILY WORK, SELF STUDY)
* **Target Variable:** `EXAM SCORE`

## Model Comparison & Evaluation
Models were evaluated on an 80/20 train-test split using Root Mean Squared Error (RMSE) and R² Score metrics:

| Model Name | RMSE | R² Score |
| :--- | :--- | :--- |
| **Linear Regression (Baseline)** | **1.538** | **0.9934** |
| **Random Forest Regressor (Advanced)** | 3.125 | 0.9728 |

## Key Insights
1. **Self-Study Impact:** `SELF STUDY` hours show the strongest positive correlation (+0.975) with final exam scores.
2. **Stress & Screen Time:** `STRESS` (-0.960) and `VIDEO GAMES` hours (-0.749) serve as strong negative predictors of academic output.
3. **Consistency Matters:** High attendance (>85%) and satisfactory daily work completion establish a protective baseline against failing grades.

## How to Run
1. Open Google Colab or Jupyter Notebook.
2. Upload `student.csv`.
3. Run `student_analysis.ipynb` sequentially.
