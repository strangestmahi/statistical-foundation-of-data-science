# Practical 7: Regression Analysis and ANOVA using Python

## Aim
To perform regression analysis and ANOVA on the Teaching Ratings dataset to study the relationship between teaching evaluation, gender, beauty scores and age groups.

## Libraries Used
- **Pandas:** For data loading and manipulation.
- **NumPy:** For numerical operations.
- **Statsmodels:** For regression analysis and statistical modelling.
- **SciPy:** For statistical functions.
- **Statsmodels ANOVA:** For performing analysis of variance.

## Dataset
The Teaching Ratings dataset is obtained from IBM Skills Network. It contains information about 463 professors, including age, gender, beauty scores, teaching evaluation and tenure.

## Description

The following operations were performed:

1. Imported the required Python libraries.
2. Loaded the Teaching Ratings dataset using Pandas.
3. Displayed the dataset's shape, column names and first five rows.
4. Performed linear regression to analyse the relationship between gender and teaching evaluation scores.
5. Calculated the gender regression coefficient, t-statistic and p-value.
6. Generated descriptive statistics for professor age.
7. Divided professors into Young, Middle-aged and Older age groups using `pd.cut()`.
8. Performed one-way ANOVA to compare beauty scores across different age groups.
9. Performed linear regression to examine the relationship between beauty scores and teaching evaluation scores.
10. Calculated the R-squared value to measure the explanatory power of the regression model.

## Important Results

| Measurement | Result |
|---|---:|
| Total observations | 463 |
| Gender coefficient | -0.1680 |
| Gender p-value | 0.00124 |
| ANOVA F-statistic | 17.5976 |
| ANOVA p-value | 4.3225 × 10⁻⁸ |
| Beauty coefficient | 0.1330 |
| Beauty R-squared | 0.0357 |
| Beauty regression p-value | 0.00004247 |

### Observations

- **Gender Regression:** Gender has a statistically significant association with teaching evaluation scores.
- **ANOVA:** Mean beauty scores differ significantly among the three age groups.
- **Beauty Regression:** Beauty score has a positive and statistically significant relationship with teaching evaluation.
- **R-squared:** Beauty score explains approximately 3.57% of the variation in teaching evaluation scores.

## Tools Used
- Python
- Google Colab
- Pandas
- NumPy
- Statsmodels
- SciPy

## Conclusion
Successfully performed regression analysis and ANOVA on the Teaching Ratings dataset. Learned how to build regression models, interpret coefficients, calculate R-squared values, divide numerical data into groups and perform ANOVA to identify significant differences between groups.
