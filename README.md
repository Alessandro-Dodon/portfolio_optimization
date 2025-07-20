# Portfolio Optimization

This repository contains a comprehensive portfolio optimization project completed during my Master's in Quantitative Finance at USI Lugano. It combines theoretical insights from Modern Portfolio Theory with practical applications using real stock market data. The project explores both analytical and simulation-based techniques, such as efficient frontier optimization and Monte Carlo simulations.

## Overview

The primary objective is to evaluate the risk-return profiles of Dow Jones Industrial Average (DJIA) stocks through:

- **Data Collection**: Historical data of DJIA stocks and index from Yahoo Finance between August 31, 2020, and February 26, 2024.  
- **Log Returns and Correlation Analysis**: Use of log returns to compute summary statistics, annualized volatility, and the correlation matrix.  
- **GARCH Modeling**: Estimating and visualizing DJIA volatility using a GARCH(1,1) model.  
- **Efficient Frontier (Markowitz Optimization)**: Analytical computation of the efficient frontier with and without short-selling, and identification of tangency and minimum-variance portfolios.  
- **Monte Carlo Simulations**:  
  - *Experiment 1*: Approximating the efficient frontier using simulated portfolios.  
  - *Experiment 2*: Analyzing the effect of diversification across multiple random subsets.  
- **Weight Generation Techniques**: Use of truncated normal (shorting allowed) and Dirichlet distributions (long-only) for sampling portfolio weights.  
- **Visualizations and Tables**: Extensive visualization of results with heatmaps, scatter plots, efficient frontier curves, and comparison tables.

## Files

**`portfolio_optimization.ipynb`**  
The main notebook performing the entire workflow, from data preparation to analytical and simulation-based optimization. It includes descriptive comments and inline Markdown sections to support theoretical explanations.

**`plots/`**  
This folder contains all generated visual outputs used in the analysis:

- `corr_matrix.png` – Annualized correlation matrix heatmap of log returns.  
- `efficient_frontier.png` – Efficient frontier with and without short-selling.  
- `monte_carlo.png` – First Monte Carlo experiment: approximating the efficient frontier.  
- `monte_carlo_subsets_long.png` – Second Monte Carlo experiment (long-only portfolios).  
- `monte_carlo_subsets_short.png` – Second Monte Carlo experiment (short-selling allowed).  

## Results Example

Below is a selection of visualizations that illustrate key findings:

**Annualized Correlation Matrix**
![Correlation Matrix](plots/corr_matrix.png)

**Efficient Frontier (Analytical)**
![Efficient Frontier](plots/efficient_frontier.png)

**Monte Carlo Simulation: Full Universe**
![Monte Carlo](plots/monte_carlo.png)

**Monte Carlo (Long-Only Subsets)**
![MC Long Subsets](plots/monte_carlo_subsets_long.png)

**Monte Carlo (Shorting Subsets)**
![MC Short Subsets](plots/monte_carlo_subsets_short.png)

## User Guide

1. **Setup**:  
   - Clone the repository (Recommended):  
     ```bash
     git clone https://github.com/Alessandro-Dodon/portfolio_optimization.git
     cd portfolio_optimization
     ```
   - Download as ZIP (Alternative):  
     Click the **"Code"** button at the top of the repository page, select **"Download ZIP"**, and extract the contents.

2. **Execution**:  
   - Open the `portfolio_optimization.ipynb` notebook in your preferred Jupyter environment.  
   - Run all cells sequentially to execute the analysis.  
   - An internet connection is required to fetch data from Yahoo Finance.  

3. **Dependencies**:  
   - All required packages are listed and imported in the notebook.  
   - If any are missing, simply uncomment the relevant `pip install` lines in the notebook.

## Contact

For questions, feedback, or suggestions, feel free to reach out via email at alessandro.dodon@usi.ch.  
You can also find my LinkedIn profile through my GitHub bio.
