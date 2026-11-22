# Practical 11: Sunspot Analysis using Gamma Distribution and MCMC

## Aim
To analyze historical sunspot data, study its distribution, and estimate Gamma distribution parameters using the Metropolis-Hastings Markov Chain Monte Carlo (MCMC) algorithm.

## Dataset
**Monthly Sunspot Numbers Dataset**

Source: SILSO – World Data Center for the Production, Preservation and Dissemination of the International Sunspot Number.

- Total observations: 3,239
- Time period: 1749–2018
- Data frequency: Monthly
- Number of time blocks: 23
- Block duration: 12 years (144 months)

## Libraries Used
- Pandas
- NumPy
- Matplotlib
- SciPy

## Steps Performed
1. Imported the required Python libraries.
2. Loaded the monthly sunspot dataset.
3. Sorted the data according to date.
4. Divided the dataset into consecutive 12-year blocks.
5. Identified zero and positive sunspot observations.
6. Calculated descriptive statistics for each time block.
7. Created a time-series plot to visualize historical sunspot activity.
8. Generated a histogram to study the distribution of sunspot numbers.
9. Initialized a Gamma distribution using shape parameter alpha = 4 and scale parameter beta = 10.
10. Implemented the Metropolis-Hastings MCMC algorithm to estimate Gamma distribution parameters.
11. Removed burn-in samples and calculated posterior estimates.
12. Created trace plots and histograms to examine MCMC sampling behaviour.
13. Calculated 95% credible intervals for alpha and beta.
14. Repeated MCMC analysis for all 23 time blocks.
15. Visualized changes in estimated parameters and Gamma means across different time periods.

## Results

| Parameter | Result |
|---|---:|
| Total Observations | 3,239 |
| Zero Observations | 67 |
| Positive Observations | 3,172 |
| Proportion of Zero Observations | 0.0207 |
| Number of Time Blocks | 23 |
| Samples per MCMC Chain | 12,000 |
| Burn-in Samples Removed | 2,400 |
| Remaining Samples | 9,600 |
| Acceptance Rate (First Block) | 47.33% |

### Gamma Distribution Estimates (First Block)

| Parameter | Posterior Mean |
|---|---:|
| Alpha (Shape) | 1.9882 |
| Beta (Scale) | 37.4525 |
| Estimated Gamma Mean | 74.4649 |

### 95% Credible Intervals

| Parameter | Lower Limit | Upper Limit |
|---|---:|---:|
| Alpha | 1.6145 | 2.4334 |
| Beta | 29.5543 | 47.1567 |

## Conclusion
Historical sunspot data was successfully analyzed using time-series visualization and Gamma distribution modelling. The Metropolis-Hastings MCMC algorithm was used to estimate the shape and scale parameters of the Gamma distribution. The analysis was extended across 23 consecutive 12-year blocks to study changes in sunspot activity over time. The results show that the estimated Gamma parameters and mean sunspot activity vary across different historical periods.
