# Portfolio Optimization

This repository contains a portfolio optimization project completed during my Master's in Quantitative Finance at USI Lugano. It applies both analytical and simulation-based techniques to explore optimal asset allocation using DJIA data.

## Overview

The notebook is structured around four core components:

- **Summary Statistics & Volatility Modeling**  
  Daily log returns of DJIA constituents are analyzed, with annualized statistics and a GARCH(1,1) model applied to the DJIA index for volatility estimation.

- **Efficient Frontier Construction**  
  Analytical frontiers are computed both with and without short-selling, highlighting the role of constraints in shaping optimal portfolios.

- **Monte Carlo Experiment 1**  
  Random portfolios are generated using truncated normal and Dirichlet distributions to approximate the efficient frontier and explore the limits of simulation vs. analytical methods.

- **Monte Carlo Experiment 2**  
  Multiple random subsets of stocks are used to show how diversification influences return–risk characteristics and overall portfolio efficiency.

## Files

**`portfolio_optimization.ipynb`**  
The main notebook containing the entire workflow, from data download and preprocessing to analytical modeling and simulation results.

**`plots/`**  
Folder containing all generated figures used in the analysis and summary.

## Results Example

**Annualized Correlation Matrix of DJIA Stocks**  
Visualizes how strongly assets move together based on log returns.

![Correlation Matrix](plots/corr_matrix.png)

**Efficient Frontier with and without Short-Selling**  
Analytical result from constrained portfolio optimization.

![Efficient Frontier](plots/efficient_frontier.png)

**Monte Carlo Simulation: Full Universe**  
Shows how simulated portfolios approximate the analytical efficient frontier using generated weights.

![Monte Carlo](plots/monte_carlo.png)

**Monte Carlo Experiment 2: Long-Only Portfolios from Random Subsets**  
Highlights variability across 6 different random subsets under long-only constraints.

![Monte Carlo Subsets Long](plots/monte_carlo_subsets_long.png)

**Monte Carlo Experiment 2: Portfolios with Short Selling from Random Subsets**  
Same 6 subsets as above but allowing short-selling to illustrate impact on efficiency.

![Monte Carlo Subsets Short](plots/monte_carlo_subsets_short.png)

## User Guide

1. **Setup**  
   - Clone the repository (Recommended):  
     ```bash
     git clone https://github.com/Alessandro-Dodon/portfolio_optimization.git
     cd portfolio_optimization
     ```
   - Or download as ZIP and extract locally.

2. **Execution**  
   - Open `portfolio_optimization.ipynb` in Jupyter Lab, VS Code, or Anaconda.  
   - Run all cells to reproduce the analysis.  
   - An internet connection is required to download data from Yahoo Finance.

3. **Dependencies**  
   - All required libraries are listed in the notebook.  
   - Use the `pip install` lines provided if any packages are missing.

## Contact

For questions or feedback, feel free to email me at **alessandro.dodon@usi.ch**.  
You can also find my LinkedIn profile via my GitHub bio.
