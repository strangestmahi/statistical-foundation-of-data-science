# Statistics for Data Science Practical (M4): Bakery Order Quantity

**Name:** Mahi Sharma
**Reg. ID:** GF202460306
**University:** Shoolini University, B.Tech

## About
This practical uses Monte Carlo simulation to solve the newsvendor problem
for a bakery that makes celebration cakes every morning.

- Cost to make one cake: ₹150
- Selling price: ₹400
- Unsold cakes are sold to a canteen at ₹50
- Daily demand is Normal(80, 20), rounded and never below 0

I simulated 20,000 days of demand with a fixed random seed so the results
can be checked:

```python
rng = np.random.default_rng(16)
demand = np.maximum(np.round(rng.normal(80, 20, 20000)), 0).astype(int)
```

## What the code does
1. Simulates 20,000 days of demand.
2. Finds the expected daily profit for every order quantity Q from 50 to 130.
3. Plots expected profit against Q and marks the best Q.
4. Finds the theoretical best Q using the critical ratio (p - c) / (p - s)
   and the normal quantile, and compares it with the simulation.
5. For the best Q, finds the probability of running out of cakes and the
   average number of leftover cakes.
6. Extra: repeats the analysis with a salvage value of ₹0.

## Results
| Quantity | Salvage = ₹50 | Salvage = ₹0 |
|---|---|---|
| Critical ratio | 0.7143 | 0.6250 |
| Theoretical best Q | 91.32 | 86.37 |
| Best Q (simulation) | 91 | 86 |
| Expected daily profit | ₹17,637.85 | ₹16,982.72 |
| Probability of running out | 0.2812 | 0.3746 |
| Average leftover cakes | 14.61 | 11.29 |

## Conclusion
- The best Q (91) is higher than the average demand (80) because running out
  of a cake loses ₹250 of profit, but a leftover cake loses only ₹100. Missing
  a sale costs more than a leftover, so the bakery should bake a few extra.
- The simulation (Q = 91) and the theory (Q* = 91.32) give the same answer.
- If the canteen stops buying leftovers, the best Q falls to 86 and the
  expected profit drops by about ₹655, because leftovers now cost more.

## Libraries used
numpy, pandas, scipy, matplotlib

## How to run
1. Open `M4_notebook.ipynb` in Google Colab or Jupyter Notebook.
2. Run all cells (Runtime → Run all).
