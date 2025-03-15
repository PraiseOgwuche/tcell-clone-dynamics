# T Cell Clone Dynamics: Modeling CD8+ T Cell Persistence After mRNA Neoantigen Vaccination

## Project Overview
This repository contains computational models and analysis of T cell clone dynamics following mRNA neoantigen vaccination, based on the findings from Sethna et al.'s 2024 paper "RNA neoantigen vaccines prime long-lived CD8+ T cells in pancreatic cancer." The project implements a stochastic simulation framework to model how vaccine-induced CD8+ T cell clones expand, contract, and transition between phenotypic states over time.

## Repository Structure
- `/data`: Directory for simulated data
- `/figures`: Visualizations of model outputs
- `tcell_clone_dynamics.ipynb`: Jupyter notebook containing the model implementation
- `requirements.txt`: Python dependencies

## Key Features
- Simulation of T cell clone dynamics with realistic biological parameters
- Modeling of phenotypic transitions between proliferative, effector, and TRM-like states
- Analysis of boost effects on clone half-life and persistence
- Correlation of T cell persistence with simulated clinical outcomes

## Immunological Concepts Addressed
This project addresses four key areas of computational immunology:
1. **Cellular Immunology**: Models different CD8+ T cell phenotypes and their evolution over time
2. **Systems Immunology**: Implements a systems-level approach to tracking clone dynamics
3. **Immune Response**: Captures how T cells respond to vaccination triggers and transition through states
4. **Translational Immunology**: Connects T cell persistence to clinical outcomes

## Key Findings
- A single boost dose increases T cell clone half-life by approximately 8.3x
- 78.8% of boosted clones persist beyond the critical 3-year PDAC recurrence window
- T cells transition from predominantly proliferative during expansion to mostly TRM-like in memory phase
- Clone persistence correlates positively with recurrence-free probability (correlation: 0.46)

## How to Run the Simulation
1. Install dependencies: `pip install -r requirements.txt`
2. Open and run `tcell_clone_dynamics.ipynb` in Jupyter

## Methods
The model implements:
- Stochastic simulation of clone frequencies over time
- Exponential decay models for clone contraction
- Markov transition matrices for phenotype changes
- Parameter estimation based on published findings

## References
- Sethna, Z., Guasp, P., Reiche, C., et al. (2024). RNA neoantigen vaccines prime long-lived CD8+ T cells in pancreatic cancer. Nature. https://doi.org/10.1038/s41586-024-08508-4

## License
MIT License

## Contact
For questions or collaboration, please open an issue on this repository.