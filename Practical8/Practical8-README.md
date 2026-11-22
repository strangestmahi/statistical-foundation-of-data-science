# Practical 8: Decision Tree Classification using Python

## Aim
To implement a Decision Tree Classifier using Python and analyze its performance using entropy, information gain, and the Gini Index.

## Dataset
**Pima Indians Diabetes Dataset**

The dataset contains information about patients and their diabetes outcomes.

- Total records: 768
- Total columns: 9
- Independent variables: 8
- Target variable: Outcome
- Outcome 0: No Diabetes
- Outcome 1: Diabetes

## Libraries Used
- Pandas
- NumPy
- Matplotlib
- Scikit-learn

## Steps Performed
1. Imported the required Python libraries.
2. Loaded the Pima Indians Diabetes dataset.
3. Checked the dataset structure and missing values.
4. Separated independent variables and the target variable.
5. Divided the dataset into training and testing sets using an 80:20 ratio.
6. Trained a Decision Tree Classifier using the entropy criterion.
7. Evaluated the model using accuracy, classification report, and confusion matrix.
8. Visualized the decision tree.
9. Calculated entropy, information gain, and the Gini Index.
10. Compared entropy-based and Gini-based decision trees.
11. Visualized feature importance and outcome distribution.

## Results

| Parameter | Result |
|---|---:|
| Total Records | 768 |
| Training Records | 614 |
| Testing Records | 154 |
| Entropy-based Model Accuracy | 70.13% |
| Gini-based Model Accuracy | 72.73% |
| Dataset Entropy | 0.9331 |
| Dataset Gini Index | 0.4544 |
| Root Feature | Glucose |
| Root Threshold | 154.5 |

### Feature Importance
- Glucose: Highest information gain (0.1146).
- BMI: Second highest information gain (0.0801).
- Pregnancies: 0.0610.
- Age: 0.0514.

### Confusion Matrix
The confusion matrix for the entropy-based model was:

| | Predicted: No Diabetes | Predicted: Diabetes |
|---|---:|---:|
| Actual: No Diabetes | 80 | 20 |
| Actual: Diabetes | 26 | 28 |

## Conclusion
The Decision Tree Classifier was successfully implemented using the Pima Indians Diabetes Dataset. Entropy and Gini Index were used to measure impurity and compare decision tree models. Glucose was identified as the root feature with a threshold of 154.5. The Gini-based model achieved 72.73% accuracy, performing slightly better than the entropy-based model on the test dataset.
