# Student Performance Analysis

## Objective
Analyze student data to predict academic success (final grades and pass/fail) and identify key influencing factors.

## Dataset
395 student records with demographic (e.g., age, gender) and academic features (e.g., G1, G2 grades, study time, past failures, absences), including final grade G3 and a derived pass/fail indicator.

## Methods
- **Exploratory Data Analysis (EDA):** Visualize distributions and relationships.
- **Linear Regression:** Predict final grade (G3) from prior scores and behaviors.
- **Logistic Regression:** Predict pass/fail status.
- **Error Analysis:** Inspect misclassifications to understand model weaknesses.

## Key Findings
- **Prior Performance Matters:** G1 and G2 scores are the dominant predictors of G3 and pass likelihood.
- **Impact of Failures:** Each past failure significantly lowers the chance of passing.
- **Limited Effect of Behaviors:** Study time and absences show minimal independent effect once prior grades are considered.
- **Model Performance:** Achieved ~87% accuracy on pass/fail classification, with high precision for passing students.
- **Model Weakness:** Struggles with borderline/improving students not well captured by past grades.

## Tools
Python (pandas, numpy), matplotlib, seaborn, scikit-learn
