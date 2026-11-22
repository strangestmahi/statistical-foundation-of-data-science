# Practical 6: Hypothesis Testing and Correlation Analysis using Python

## Aim
To perform different statistical tests, including T-test, ANOVA, Chi-Square test and Pearson Correlation, on the Teaching Ratings dataset using Python.

## Libraries Used
- **NumPy:** For numerical operations.
- **Pandas:** For data manipulation and analysis.
- **SciPy:** For performing statistical tests.
- **Matplotlib:** For creating graphs and visualizations.

## Dataset
The Teaching Ratings dataset is obtained from IBM Skills Network. It contains information about professors, including age, gender, beauty scores, teaching evaluation, tenure and course details.

## Description

The following operations were performed:

1. Imported the required Python libraries.
2. Loaded the Teaching Ratings dataset using Pandas.
3. Displayed the first five rows and column names.
4. Performed an independent two-sample T-test to compare teaching evaluation scores between male and female instructors.
5. Grouped professors into Young, Middle and Older age categories using `pd.cut()`.
6. Performed a one-way ANOVA test to compare beauty scores across different age groups.
7. Created a contingency table to compare tenure status and gender.
8. Performed a Chi-Square test to examine the association between tenure and gender.
9. Calculated the Pearson correlation coefficient between beauty scores and teaching evaluation scores.
10. Checked the statistical significance of the correlation.
11. Created a scatter plot to visualize the relationship between beauty scores and evaluation scores.

## Important Results

| Statistical Test | Result |
|---|---|
| Male mean evaluation | 4.0690 |
| Female mean evaluation | 3.9010 |
| T-statistic | 3.2667 |
| T-test p-value | 0.00118 |
| ANOVA F-statistic | 15.6552 |
| ANOVA p-value | 0.0000002645 |
| Chi-Square statistic | 2.2068 |
| Chi-Square p-value | 0.1374 |
| Degrees of freedom | 1 |
| Correlation coefficient | 0.1890 |
| Correlation p-value | 0.00004247 |

### Observations

- **T-test:** Teaching evaluation scores differ significantly between male and female instructors at the 5% significance level.
- **ANOVA:** Beauty scores differ significantly across the three age groups.
- **Chi-Square test:** No statistically significant association was found between tenure status and gender.
- **Correlation:** Beauty score and teaching evaluation have a weak positive and statistically significant relationship.

## Tools Used
- Python
- Google Colab
- Pandas
- NumPy
- SciPy
- Matplotlib

## Conclusion
Successfully performed hypothesis testing and correlation analysis on the Teaching Ratings dataset. Learned how to apply T-test, ANOVA, Chi-Square test and Pearson correlation to analyse relationships and differences between variables.
