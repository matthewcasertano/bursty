# Neural Autopilot Model: Parameter Space Analysis

This repository contains parameter analysis code for the Neural Autopilot model, developed as part of research on power laws in human behavior in the Colin Camerer lab at Caltech.

## Author Contribution
This repository represents my contribution to the broader research project. The parameter space analysis, ground truth recovery implementation, and visualization code were developed by me as part of collaborative work with Sean Hu and the Camerer lab team.

## Working Paper Citation
Hu, S., Kalburge, I., Ho, H., Kukavica, A., & Camerer, C. (2025). *Power laws in human individual behavior: Improved statistical tests and novel neural autopilot explanation*. Working paper.

## Repository Contents

- **`run.ipynb`** - Main analysis notebook containing four key tasks (my contribution, with some code adapted from previous work)
- **`analyze.ipynb`** - Additional visualization and parameter space analysis (my contribution)
- **`parameter_space_results.csv`** - Full parameter space simulation results
- **`archive_parameter_space_results.csv`** - Backup of complete results from HPC runs
- **`VariationOf_0320_2025.csv`** - Supporting data file
- **`slides_excerpt.pdf`** - Presentation slides (34-40) covering my parameter analysis contributions

## Analysis Overview

### Main Tasks (run.ipynb)

**Task A: Ground Truth Recovery for Empirical Parameter Sets**
- Simulate and estimate parameters for four datasets (Gym, Moment, Weibo, Zearn)
- Compare initial vs. estimated parameters to validate model recovery

**Task B: Full Parameter Space Simulation** 
- Comprehensive ground truth recovery across parameter combinations
- Results saved to `parameter_space_results.csv`

**Task C: Simulation Limitations Analysis**
- Investigation of high δ/low λ parameter regions
- Analysis and visualization of NaN simulation cases

**Task D: Habit Mode Analysis**
- Measurement of habit mode characteristics for empirical parameter sets
- Analysis of time spent in habit mode and choice patterns

### Additional Analysis (analyze.ipynb)
- Parameter space visualization and stability analysis
- NaN case investigation with heatmap visualizations  
- Cumulative distribution function analysis
- Grid-based parameter exploration

## Usage

To run the analysis quickly for testing:
1. Change `NUM_TRIALS` in the first cell of `run.ipynb` to a smaller value (e.g., 50)
2. Execute the notebook cells sequentially

For full analysis, use the default `NUM_TRIALS = 1500` (computationally intensive).

## Data
The full parameter space results were generated using high-performance computing with 1500 trials per parameter combination. The archive file preserves these complete results for reproducibility.
