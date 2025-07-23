# Modeling the Reverse Water–Gas Shift (RWGS) Reaction with Machine Learning

This repository accompanies the manuscript **“Modeling of a Reverse Water–Gas Shift Reactor with Machine Learning”** by Komatz _et al._ It compares multiple machine-learning approaches for predicting CO₂ conversion (**X(CO₂)**) and CO selectivity (**S(CO)**) under varied reactor conditions.

## Overview

- **Challenge:** The RWGS reaction network involves competing pathways and both kinetic and thermodynamic limitations.  
- **Data:** Simulated reactor outputs across:  
  - Temperature (`Tout`, 400–800 °C)  
  - Pressure (`pset`, 1–30 bar)  
  - H₂/CO₂ feed ratio  
  - Gas Hourly Space Velocity (`GHSV`)  
- **Objectives:**  
  1. Benchmark simple regressors (Linear, Lasso, Decision Tree)  
  2. Evaluate ensembles (Random Forest, Gradient Boosting)  
  3. Train artificial neural networks (ANN)  
  4. Interpret models with SHAP analysis

## Installation

```bash
git clone https://github.com/yourusername/rwgs-ml-modeling.git
cd rwgs-ml-modeling

# (Optional) Create and activate a virtual environment
python3 -m venv venv
source venv/bin/activate

pip install --upgrade pip
pip install -r requirements.txt

## Citation
@article{Komatz2025,
  author    = {Enzo Komatz and Marion Andritz and Markus Lehner and Christoph Markowitsch},
  title     = {Modeling of a Reverse Water–Gas Shift Reactor with Machine Learning},
  journal   = {High Impact Journal},
  year      = {2025},
  doi       = {10.xxx/hi-2025-001},
}
