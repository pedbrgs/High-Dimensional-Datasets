# High-Dimensional Data Collection

**Author:** [Pedro Vinícius A. B. Venâncio](https://www.linkedin.com/in/pedbrgs/)<sup>1</sup> <br />

***

## About

This repository provides a curated collection of high-dimensional datasets designed for performance evaluation experiments in machine learning.

## Repository Structure

This repository is organized into two main folders:

- [collection/](https://github.com/pedbrgs/High-Dimensional-Datasets/tree/main/collection): contains the curated list of datasets included in the benchmarking suite.
- [pipeline/](https://github.com/pedbrgs/High-Dimensional-Datasets/tree/main/pipeline): contains the preprocessing pipelines implemented as Jupyter notebooks, ensuring reproducibility and transparency.

Both directories are organized by machine learning task (e.g., binary classification, multiclass classification, clustering, regression, and others).

## Dataset Schema

Each dataset in this collection adheres to the conventions below:

- **Predictor variables** are indexed sequentially with integer column names ranging from `0` to `N-1`, where `N` is the total number of predictive features.
- The **label column** is named after the original response variable from the source dataset.
- The **`subset` column** identifies whether an observation belongs to the training or test partition (values: `train` or `test`).
- When the original dataset does not provide a predefined split, the data is randomly partitioned into **70% training** and **30% test** subsets as part of the preprocessing pipeline.

This standardized format ensures uniform data handling across all datasets and experimental workflows.

### Example

The table below illustrates the standardized structure using a random sample with up to 10 features (0 to 9) and 10 observations:

| 0    | 1    | 2    | 3    | 4    | 5    | 6    | 7    | 8    | 9    | label | subset |
|------|------|------|------|------|------|------|------|------|------|-------|--------|
| 1.32 | 0.45 | 2.11 | 0.98 | 1.56 | 0.12 | 3.45 | 1.08 | 0.77 | 2.01 | 1     | train  |
| 0.87 | 1.23 | 1.98 | 0.56 | 0.44 | 1.76 | 2.34 | 0.67 | 1.45 | 1.89 | 0     | train  |
| 1.11 | 0.94 | 2.56 | 1.34 | 0.89 | 0.65 | 3.01 | 1.22 | 0.54 | 2.15 | 1     | train  |
| 0.45 | 1.56 | 1.23 | 0.78 | 1.12 | 1.04 | 2.88 | 0.91 | 1.33 | 1.47 | 0     | train  |
| 1.76 | 0.88 | 2.01 | 1.09 | 0.67 | 0.32 | 3.21 | 1.15 | 0.81 | 2.30 | 1     | train  |
| 0.92 | 1.14 | 1.67 | 0.63 | 1.01 | 0.89 | 2.54 | 0.84 | 1.26 | 1.58 | 0     | train  |
| 1.25 | 0.51 | 2.34 | 1.21 | 0.73 | 0.47 | 3.10 | 1.05 | 0.69 | 2.09 | 1     | train  |
| 0.68 | 1.31 | 1.45 | 0.82 | 1.18 | 1.12 | 2.66 | 0.79 | 1.41 | 1.63 | 0     | test   |
| 1.03 | 0.76 | 2.19 | 1.02 | 0.95 | 0.28 | 3.00 | 1.11 | 0.72 | 2.18 | 1     | test   |
| 0.59 | 1.42 | 1.88 | 0.71 | 1.06 | 0.97 | 2.73 | 0.86 | 1.37 | 1.52 | 0     | test   |

## Contributions

Contributions are welcome!
If you want to add new datasets, improve documentation, or provide loaders, feel free to open a pull request.
