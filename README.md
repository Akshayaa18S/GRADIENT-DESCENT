# GRADIENT-DESCENT
# Gradient Descent vs. Linear Search

## Overview
This project compares two optimization techniques for finding the best slope in a simple linear regression problem:
1. **Linear Search** (Brute-force approach)
2. **Gradient Descent** (Iterative optimization)

The dataset is synthetically generated with noise, and we analyze how each method finds the best-fitting slope.

## File Structure
- **Gradient Descent.py** → Python script containing the implementation of both methods, plots, and results.
- **README.md** → This file explaining the project.

## Methods Explained
### 1. Linear Search
- Scans a predefined range of slope values and calculates the Mean Squared Error (MSE) for each.
- Selects the slope with the lowest MSE as the optimal solution.
- Quick and simple but inefficient for large datasets.

### 2. Gradient Descent
- Iteratively updates the slope and intercept using gradients of the loss function.
- Requires setting a **learning rate** and **number of epochs**.
- More efficient for large datasets but depends on hyperparameters.

## Results & Comparison
| Method            | Best Slope | Final Loss | Time Taken  |
|------------------|------------|-------------|-------------|
| Linear Search    | 2.7879      | 0.9316       | 0.001462 sec |
| Gradient Descent | 3.3697      | 6.6211       | 0.001373 sec  |

- **Linear Search** is accurate but inefficient for large search spaces.
- **Gradient Descent** is scalable but sensitive to hyperparameters like learning rate.

## Visualization
- **Loss vs. Slope**: Shows how loss changes across different slopes (Linear Search).
- **Loss Convergence**: Displays how loss decreases over epochs (Gradient Descent).

## How to Run
1. Run **Gradient Descent.py** in Python.
2. The script will generate the data, optimize, and visualize results.

## Dependencies
```bash
pip install numpy matplotlib
```
