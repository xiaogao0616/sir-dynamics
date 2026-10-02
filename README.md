# SIR Dynamics

A numerical modeling experiment comparing Explicit Euler and fourth-order Runge–Kutta (RK4) methods on an SIR epidemic model.

Built for **MATH 383L: Differential Equations Lab** at UNC–Chapel Hill, Spring 2026.

## The experiment

- Implement the SIR differential equations and both numerical methods in Python.
- Compare susceptible, infected, and recovered trajectories over 30 days.
- Compare fine and coarse time steps (0.001 and 1 day).
- Measure absolute error in the infected population at day 10 against a fine-step RK4 reference.

The simulated population is 1,000, initially split into 990 susceptible and 10 infected individuals. The model uses beta = 1.87/day and gamma = 0.5/day. This is a classroom simulation, not a fit to observed UNC outbreak data.

## Files

- [383L_coding.ipynb](383L_coding.ipynb) — original notebook, unchanged.
- [report.pdf](report.pdf) — original course report, unchanged; renamed for a shorter link.

## Run locally

Use Python 3 with NumPy, Matplotlib, and Jupyter Notebook:

```sh
python -m pip install numpy matplotlib notebook
jupyter notebook 383L_coding.ipynb
```

Run all four cells in order. The notebook displays three figures and saves `Figure1_Baseline.png`, `Figure2_Stability_Comparison.png`, and `Figure3_Error_Analysis.png` in the working directory. Its plotting style requires Matplotlib 3.6 or newer.

## Context & contribution

The original group report lists **Feier Xu, Jiaying Zhang, and Xiangyi Gao**.

**Xiangyi Gao:** primary contributor to the numerical implementation, experiments, and visualization.

This repository preserves the submitted notebook and report as a course-project archive.
