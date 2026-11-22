# Practical 12 – Metropolis Algorithm and Bayesian Parameter Estimation

## Aim
To implement the Metropolis algorithm for Markov Chain Monte Carlo (MCMC), study sampling efficiency, and perform Bayesian parameter estimation for a logistic growth model.

## Libraries Used
- NumPy
- Matplotlib
- SciPy
- Pandas
- Statsmodels

## Steps Performed

1. **Target Distribution:** Created a bimodal probability distribution using a mixture of two Gaussian distributions.

2. **Metropolis Algorithm:** Implemented the Metropolis algorithm using a Gaussian random-walk proposal to generate samples from the target distribution.

3. **Burn-in and Visualization:** Removed initial burn-in samples and plotted the generated sample distribution against the theoretical probability distribution. Trace plots were also created.

4. **Proposal Step Size Analysis:** Tested different step sizes (0.5, 1.0, 2.5, 5.0 and 10.0) to study their effects on acceptance rate and sampling efficiency.

5. **Autocorrelation Analysis:** Used the Autocorrelation Function (ACF) to examine the dependence between successive samples.

6. **Effective Sample Size (ESS):** Compared the effective number of independent samples generated using different proposal step sizes.

7. **Convergence Diagnostic:** Applied the Gelman-Rubin diagnostic using four independent Markov chains to examine convergence.

8. **Deterministic Logistic Model:** Implemented the logistic growth differential equation and compared its numerical solution with the analytical solution.

9. **Noisy Data Generation:** Generated 16 observations by adding Gaussian noise to the logistic growth model.

10. **Bayesian Parameter Estimation:** Used the Metropolis algorithm to estimate the unknown growth rate (r) and carrying capacity (K) from noisy observations.

11. **Posterior Analysis:** Removed burn-in samples and plotted trace plots and posterior distributions for both parameters.

## Results

### Metropolis Algorithm
- Generated 50,000 samples with 5,000 burn-in iterations.
- The generated histogram reproduced the bimodal target distribution.
- Different proposal step sizes affected acceptance rates and sampling efficiency.
- Step size 5.0 produced the highest ESS among the tested values, with 3,670 effective samples.

### Convergence Analysis
- Four independent chains were generated.
- The R-hat value was approximately 1.0000.
- The result indicated good agreement between the chains, although additional diagnostics may be needed to confirm reliable mixing.

### Logistic Growth Model
- Initial population: 5
- Growth rate (r): 0.8
- Carrying capacity (K): 100
- The numerical solution closely matched the analytical solution.
- The maximum error was approximately 3.34 × 10⁻⁷.

### Bayesian Parameter Estimation

| Parameter | Actual Value | Estimated Mean |
|---|---:|---:|
| Growth Rate (r) | 0.8 | 0.8092 |
| Carrying Capacity (K) | 100 | 102.5179 |

**95% Credible Intervals:**
- Growth Rate (r): [0.7678, 0.8530]
- Carrying Capacity (K): [99.1268, 105.7686]

The estimated parameters were close to their actual values.

## Conclusion
The practical successfully demonstrated the Metropolis algorithm and its application in MCMC sampling. Different sampling techniques and convergence diagnostics were studied. Bayesian parameter estimation was also performed on a logistic growth model, successfully recovering the growth rate and carrying capacity from noisy observations.
