# Practical 9: K-Nearest Neighbors (KNN) Classification using Python

## Aim
To perform Exploratory Data Analysis (EDA), feature scaling, and implement the K-Nearest Neighbors (KNN) algorithm to classify Iris flower species.

## Dataset
**Iris Dataset**

The Iris dataset contains measurements of three different species of flowers.

- Total records: 150
- Total features: 4
- Target variable: Species
- Species: Setosa, Versicolor, Virginica

## Libraries Used
- Pandas
- NumPy
- Matplotlib
- Seaborn
- Scikit-learn

## Steps Performed
1. Imported the required Python libraries.
2. Loaded the Iris dataset and converted it into a Pandas DataFrame.
3. Performed Exploratory Data Analysis (EDA) using `head()`, `describe()`, and `groupby()`.
4. Separated independent features and the target variable.
5. Divided the dataset into training and testing sets using an 80:20 ratio.
6. Applied StandardScaler for feature scaling.
7. Trained a KNN classifier using K = 3.
8. Generated predictions for the test dataset.
9. Evaluated the model using a confusion matrix, accuracy score, and classification report.
10. Compared error rates for K values ranging from 1 to 20.
11. Identified the best K value based on the minimum error rate.

## Results

| Parameter | Result |
|---|---:|
| Total Records | 150 |
| Training Records | 120 |
| Testing Records | 30 |
| Initial K Value | 3 |
| Accuracy (K = 3) | 93.33% |
| Best K Value | 1 |
| Minimum Error Rate | 3.33% |
| Best Accuracy | 96.67% |

### Confusion Matrix (K = 3)

| Actual / Predicted | Setosa | Versicolor | Virginica |
|---|---:|---:|---:|
| Setosa | 10 | 0 | 0 |
| Versicolor | 0 | 10 | 0 |
| Virginica | 0 | 2 | 8 |

### Classification Report
- Setosa: Precision 1.00, Recall 1.00
- Versicolor: Precision 0.83, Recall 1.00
- Virginica: Precision 1.00, Recall 0.80
- Overall Accuracy: 93.33%

## Conclusion
The K-Nearest Neighbors algorithm was successfully implemented using the Iris dataset. Exploratory Data Analysis and feature scaling were performed before training the model. The classifier achieved 93.33% accuracy with K = 3. After comparing error rates for K values from 1 to 20, K = 1 was identified as the best value, achieving 96.67% accuracy on the test dataset.
