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

 ## Workflow

1. Data loading and cleaning  
2. Exploratory Data Analysis (EDA)  
3. Feature engineering (pass/fail label)  
4. Linear regression for final grade prediction (G3)  
5. Logistic regression for pass/fail classification  
6. Model evaluation and error analysis  

## Key Findings
- **Prior Performance Matters:** G1 and G2 scores are the dominant predictors of G3 and pass likelihood.
- **Impact of Failures:** Each past failure significantly lowers the chance of passing.
- **Limited Effect of Behaviors:** Study time and absences show minimal independent effect once prior grades are considered.
- **Model Performance:** Achieved ~87% accuracy on pass/fail classification, with high precision for passing students.
- **Model Weakness:** Struggles with borderline/improving students not well captured by past grades.

## Results Summary

- Linear Regression (G3 prediction):
  - R² score ≈ 0.78
  - Mean Absolute Error ≈ 1.34 grades

- Logistic Regression (Pass/Fail):
  - Accuracy ≈ 87%
  - Precision (Pass) ≈ 94%
  - Recall (Pass) ≈ 87%
 
## Limitations

- Behavioral features (study time, absences) have limited predictive power once prior grades are included.
- The model struggles with borderline students whose performance is improving or declining.
- Results are dataset-specific and may not generalize to other education systems.

## Tools
Python (pandas, numpy), matplotlib, seaborn, scikit-learn

## How to Run

1. Clone the repository:
   git clone https://github.com/ad-546/Student-Performance-Analysis.git

2. Install dependencies:
   pip install -r requirements.txt

3.Open the Jupyter notebook:

  jupyter notebook student_performance_analysis.ipynb   
