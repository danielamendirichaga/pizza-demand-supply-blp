# ECON 452 Final Project: Demand and Supply Estimation in the Pizza Market

This repository contains a structural empirical industrial organization project on differentiated-product competition in the pizza market. The analysis estimates demand and supply using `pyblp`, studies price endogeneity with instrumental variables, and uses the estimated model to simulate counterfactual market outcomes.

## Project Overview

The goal of the project is to analyze how product characteristics, firm behavior, and consumer heterogeneity shape market outcomes. Using product-level and agent-level data, the notebook estimates a Berry-Levinsohn-Pakes (BLP) style model of demand and supply and then applies the estimated model to answer counterfactual questions about pricing and market equilibrium.

The project is organized around several core tasks:

- explaining why instrumental variables are needed when prices are endogenous;
- interpreting the construction and role of demand and supply instruments;
- estimating a structural model of demand and marginal costs;
- recovering firm conduct and equilibrium implications under differentiated-products Bertrand competition;
- performing simulations to study how changes in market conditions affect prices, shares, and welfare-related outcomes.

## Assignment Components

The original assignment was divided into multiple questions. In project terms, those components are reflected here as:

1. **Instrumental variables and identification**: explain why price is endogenous, why BLP instruments are useful, and how the demand and supply instruments in the dataset are constructed and interpreted.
2. **Model setup and estimation**: specify the demand and supply framework, prepare the data, and estimate the structural parameters using `pyblp`.
3. **Economic interpretation**: interpret the estimated coefficients, substitution patterns, and supply-side implications of the model.
4. **Equilibrium analysis**: recover pricing implications under differentiated-products Bertrand competition and connect the estimates to observed market outcomes.
5. **Counterfactual exercises**: simulate changes in market conditions and compare resulting prices, market shares, and related economic outcomes.

## Data

The repository includes two datasets:

- `products_pizza.csv`: product-level data including market identifiers, firm identifiers, market shares, prices, product characteristics, and instruments.
- `agents_pizza.csv`: agent-level data used to model consumer heterogeneity in demand.

Together, these datasets support both estimation and counterfactual analysis in a random-coefficients discrete-choice framework.

## Methods

The empirical workflow in the notebook includes:

- instrumental variables intuition for handling price endogeneity;
- BLP-style demand estimation with heterogeneous price sensitivity;
- supply-side estimation under Bertrand competition;
- equilibrium recovery and market simulations using `pyblp`.

The notebook combines conceptual explanations with code implementation so the project can be read both as an applied econometrics assignment and as a reproducible computational analysis.

## Repository Contents

- `EIO_FP.ipynb`: main notebook containing the analysis, estimation, and counterfactual exercises.
- `EIO_FP.pdf`: exported PDF version of the notebook/report.
- `products_pizza.csv`: product-level input data.
- `agents_pizza.csv`: agent-level input data.

## Team

This project was completed by:

- Daniela Mendirichaga
- Chenny Yang
- Hanako Doerr

## How to Run

1. Install Python 3 and Jupyter Notebook.
2. Install the required packages:

```bash
pip install pyblp pandas numpy matplotlib
```

3. Open `EIO_FP.ipynb`.
4. Run the notebook cells in order from top to bottom.

## Notes

- The notebook uses relative file paths, so it should run directly from the repository root once dependencies are installed.
- Temporary files such as `.ipynb_checkpoints` and `.DS_Store` are excluded from version control.
- This README summarizes the project in original wording rather than reproducing the course handout.
