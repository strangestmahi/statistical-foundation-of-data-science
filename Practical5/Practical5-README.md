# Practical 5: Probability and Z-Test using Python

## Aim
To calculate probabilities using the Teaching Ratings dataset and perform a Z-test to test a population mean using Python.

## Libraries Used
- **Pandas:** For loading and analysing the dataset.
- **NumPy:** For numerical operations.
- **Math:** For mathematical calculations such as square root.

## Dataset
The Teaching Ratings dataset is obtained from the Rdatasets GitHub repository. It contains information about professors, including their evaluation scores and other teaching-related details.

## Description

The following operations were performed:

1. Imported the required Python libraries.
2. Loaded the Teaching Ratings dataset from GitHub using Pandas.
3. Displayed the first five rows using `head()`.
4. Calculated the probability of a professor receiving an evaluation score greater than 4.5.
5. Calculated the probability of evaluation scores lying between 3.5 and 4.2.
6. Stored the population mean, standard deviation, sample size and sample mean.
7. Calculated the Z-test statistic using the given sample information.
8. Identified the critical values for a two-tailed test at a 5% significance level.
9. Compared the calculated Z-value with the critical values.
10. Made a final decision regarding the null hypothesis.

## Important Results

| Measurement | Result |
|---|---:|
| Probability of evaluation > 4.5 | 0.1706 |
| Probability of evaluation between 3.5 and 4.2 | 0.3542 |
| Population mean (μ) | 12 |
| Population standard deviation (σ) | 5.5 |
| Sample size (n) | 36 |
| Sample mean (x̄) | 10.7 |
| Calculated Z-value | -1.4182 |
| Critical values | ±1.96 |
| Significance level | 5% |

### Hypothesis Testing Result

- **Null Hypothesis (H₀):** The population mean is equal to 12.
- **Alternative Hypothesis (H₁):** The population mean is not equal to 12.
- **Decision:** Fail to reject the null hypothesis because the calculated Z-value lies between -1.96 and +1.96.

## Tools Used
- Python
- Google Colab
- Pandas
- NumPy
- Math

## Conclusion
Successfully calculated probabilities using the Teaching Ratings dataset and performed a two-tailed Z-test. Learned how to calculate probability, determine the Z-test statistic, identify critical values and make decisions about the null hypothesis using a 5% significance level.
