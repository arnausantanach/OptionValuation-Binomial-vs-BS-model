# Option Valuation: Binomial vs. Black-Scholes 

This is a small project I developed to reaffirm the knowledge I acquired in my **Financial Derivatives and Risk Management** class.

The main idea was to take the theoretical pricing models I learned on paper and see if I could build them from scratch using Python to compare their results.

## Objectives

The project focuses on three main goals:

1.  **Implement the Multi-Step Binomial Model** to compute option prices numerically.
2.  **Implement the Black-Scholes-Merton Model** to get the exact analytical price for comparison.
3.  **Visualize the convergence** of the Binomial model towards the Black-Scholes price as we increase the number of time steps.

## A Note on the Math 

You will notice I haven't included deep mathematical derivations for the formulas used (like the up/down factors $u, d$, the risk-neutral probability $p$, or the $d_1/d_2$ terms in Black-Scholes).

Since the primary objective of this project was **implementation** rather than **theory**, I skipped the mathematical proofs to focus purely on how to translate those formulas directly into Python code.

## Tools and Libraries

* **numpy** – for vectorization and matrix operations (essential for the price tree).
* **scipy** – for the normal distribution functions in Black-Scholes.
* **matplotlib** – for visualizing the convergence graph.

## Results

I compared the two models by pricing a standard European Call Option. The final output is a convergence graph that shows the famous "sawtooth" effect—demonstrating how the Binomial price oscillates but eventually settles on the Black-Scholes price as the time steps ($N$) increase.

## Author

Project by **Arnau Santanach** 
Created as part of a personal learning journey