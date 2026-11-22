# Practical 10: Principal Component Analysis (PCA) using Python

## Aim
To perform Exploratory Data Analysis (EDA), standardize the Wine dataset, and apply Principal Component Analysis (PCA) to reduce the dimensionality of the dataset.

## Dataset
**Wine Dataset**

The Wine dataset contains chemical measurements of wines belonging to three different classes.

- Total records: 178
- Total features: 13
- Target variable: Class
- Classes: Class 0, Class 1, Class 2

## Libraries Used
- Pandas
- NumPy
- Matplotlib
- Seaborn
- Scikit-learn

## Steps Performed
1. Imported the required Python libraries.
2. Loaded the Wine dataset and converted it into a Pandas DataFrame.
3. Displayed the first five records and class names.
4. Calculated basic statistical information using `describe()`.
5. Created a boxplot to compare alcohol content across wine classes.
6. Created a scatterplot to analyze the relationship between alcohol content and color intensity.
7. Calculated and visualized the covariance matrix using a heatmap.
8. Standardized the dataset using StandardScaler.
9. Applied PCA to reduce the original 13 features to 2 principal components.
10. Calculated the explained variance ratio and total variance explained.
11. Visualized the wine classes using the first two principal components.

## Results

| Parameter | Result |
|---|---:|
| Total Records | 178 |
| Original Features | 13 |
| Wine Classes | 3 |
| Principal Components | 2 |
| Dimensionality Reduction | 13 to 2 |

### PCA Analysis
- StandardScaler was used to bring all features to a comparable scale.
- PCA transformed the original 13 features into 2 principal components.
- The explained variance ratio was calculated to measure how much information each component retained.
- A scatterplot was created to visualize the three wine classes in the reduced two-dimensional space.

## Conclusion
Exploratory Data Analysis and Principal Component Analysis were successfully performed on the Wine dataset. The dataset was standardized before applying PCA. The original 13 features were reduced to 2 principal components, making the data easier to visualize and analyze while retaining as much variance as possible in the two-dimensional representation.
