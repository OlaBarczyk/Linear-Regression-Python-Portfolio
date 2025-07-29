# 📊 Machine Learning Portfolio

> A hands-on project demonstrating the implementation of linear regression from scratch, data preprocessing, PCA (Principal Component Analysis), and visualization using a real chemical descriptors dataset.

---

## 🧠 About The Project

This project showcases the core workflow of a typical machine learning pipeline:

- Manual implementation of **Simple and Multiple Linear Regression**
- Calculation of regression metrics: **R² (coefficient of determination)** and **MSE (Mean Squared Error)**
- **Visualization** of model behavior through regression lines, residual plots, and Q-Q plots
- **PCA (Principal Component Analysis)** to reduce data dimensionality
- **Data preprocessing**: cleaning, normalization, outlier detection (3-sigma rule), feature selection
- Built-in support for **coefficient constraints** (min, max, delta values)
- Usage of `scikit-learn` for comparison

---

## 🗂️ Table of Contents

- [About The Project](#-about-the-project)
- [Dataset](#-dataset)
- [Getting Started](#-getting-started)
- [Usage Examples](#-usage-examples)
- [Visualizations](#-visualizations)
- [Built With](#-built-with)
- [License](#-license)

---

## 📁 Dataset

The dataset used is `Descriptors.xlsx`, which contains a variety of numerical chemical descriptors such as:
- Molecular Weight (`MolWt`)
- Topological Polar Surface Area (`TPSA`)
- Chi indices (`Chi0n`)
- Hydrogen acceptor counts (`NumHAcceptors`)
- Functional group indicators (e.g., `fr_benzene`)

---

## 🚀 Getting Started

### Prerequisites

Ensure you have Python 3.10+ installed along with the following libraries:

```bash
pip install numpy pandas matplotlib seaborn scikit-learn scipy openpyxl
