## 📘 Project Structure & Technical Overview

This repository implements a **synthetic FX pricing optimization engine**, designed to illustrate how margin levels affect volume, turnover and Gross Profit across multiple segments (Country × Channel × Currency × Direction).  
The goal is to model **price elasticity**, estimate **GP-maximizing margins**, and generate **executive-ready visualizations** that replicate real-world FX pricing workflows.

The project follows a full analytical pipeline:

- **Data generation**: simulation of a realistic FX environment with controlled margin distributions, demand curves, elasticity parameters and noise components.
- **Exploratory analysis**: validation of distributions, KPIs and behavioural patterns (turnover, ATV, GP%, transactions).
- **Elasticity modelling**: simplified margin bands, segment filtering and behavioural diagnostics.
- **Pricing engine**: optimal GP% selection per segment using non-linear regression, guardrails, and data-density constraints.

The structure is intentionally modular to make the methodology transparent and easy to follow.

```text
FX Pricing Optimization Engine
│
├── 📓 notebooks/
│   ├── 01_data_simulation.ipynb
│   ├── 02_explploratory_analysis.ipynb
│   ├── 03_margin_elasticity.ipynb
│   └── 04_pricing_optimization_engine.ipynb
│
├── 📂 data/
│   └── synthetic_pricing_daily.csv
│
└── 📊 output/
    └── pricing_engine/
