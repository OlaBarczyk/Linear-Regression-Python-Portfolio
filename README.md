# Linear - Regression - Python Portfolio

> A hands-on project demonstrating the implementation of linear regression from scratch, data preprocessing, PCA (Principal Component Analysis), and visualization using a real chemical descriptors dataset.

---

## About The Project

This project showcases the core workflow of a typical machine learning pipeline:

- Manual implementation of **Simple and Multiple Linear Regression**
- Calculation of regression metrics: **R² (coefficient of determination)** and **MSE (Mean Squared Error)**
- **Visualization** of model behavior through regression lines, residual plots, and Q-Q plots
- **PCA (Principal Component Analysis)** to reduce data dimensionality
- **Data preprocessing**: cleaning, normalization, outlier detection (3-sigma rule), feature selection
- Built-in support for **coefficient constraints** (min, max, delta values)
- Usage of `scikit-learn` for comparison

---

## Table of Contents

- [About The Project](#about-the-project)
- [Dataset](#dataset)
- [Getting Started](#getting-started)
- [Usage Examples](#usage-examples)
- [Visualizations](#visualizations)
- [Built With](#built-with)
- [License](#license)

---

## Dataset

The dataset used is `Descriptors.xlsx`, which contains a variety of numerical chemical descriptors such as:

- Molecular Weight (`MolWt`)
- Topological Polar Surface Area (`TPSA`)
- Chi indices (`Chi0n`)
- Hydrogen acceptor counts (`NumHAcceptors`)
- Functional group indicators (e.g., `fr_benzene`)

---

## Getting Started

### Prerequisites

Ensure you have Python 3.10+ installed along with the following libraries:

```bash
pip install numpy pandas matplotlib seaborn scikit-learn scipy openpyxl
git clone https://github.com/OlaBarczyk/Machine-Learning-Portfolio.git
cd Machine-Learning-Portfolio
Make sure the file Descriptors.xlsx is in the same folder as MyFirstNotebook.ipynb.
```
Open MyFirstNotebook.ipynb in Jupyter Notebook or VS Code with the Jupyter extension.

Run all cells sequentially to see data preprocessing, PCA, visualizations, and regression models in action.
## Usage Examples
## Simple Linear Regression
X = np.array([[1], [2], [3], [4], [5]])
y = np.array([2, 4, 5, 4, 5])
model = MyLinearRegression()
model.fit(X, y)
model.plot(X, y)

## Multiple Linear Regression
X_multi = np.random.rand(100, 2) * 100
y_multi = 3 * X_multi[:, 0] + 2 * X_multi[:, 1] + np.random.randn(100) * 10
regression_multi = RegressionModel(X_multi, y_multi)
regression_multi.fit()
regression_multi.plot_residuals()
regression_multi.plot_qq()

## Visualizations
The following visualizations are generated using matplotlib and seaborn:

Boxplots before and after normalization for:

MolWt, Chi0n, TPSA, NumHAcceptors, fr_benzene

Histograms before and after normalization

Scatter plots for each pair of selected variables

PCA projection (2D) with explained variance printed

Regression line for single-variable model

Residual plots for model diagnostics

Q-Q plot to check residual normality

All plots are displayed within the notebook.

## Built With

- [NumPy](https://numpy.org/)
- [Pandas](https://pandas.pydata.org/)
- [Matplotlib](https://matplotlib.org/)
- [Seaborn](https://seaborn.pydata.org/)
- [scikit-learn](https://scikit-learn.org/)
- [SciPy](https://scipy.org/)
- [Jupyter Notebook](https://jupyter.org/)


## License
Distributed under the MIT License. See LICENSE for more information.

## Acknowledgements

- [Best README Template](https://github.com/othneildrew/Best-README-Template)
- [Python Graph Gallery](https://python-graph-gallery.com/)


