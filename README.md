# Intro-to-Data-Science-Project-3


# Sunspot Data Forecasting Project

This project focuses on forecasting sunspot activity over time using Facebook's Prophet library. It includes detailed forecasting for daily, monthly, and yearly intervals, showcasing the capabilities of time series analysis for scientific and astronomical data.

---

## Table of Contents

1. [Introduction](#introduction)
2. [Features](#features)
3. [Project Structure](#project-structure)
4. [Data Sources](#data-sources)
5. [Requirements](#requirements)
6. [Usage](#usage)
7. [Results](#results)
8. [Acknowledgements](#acknowledgements)

---

## Introduction

Sunspots are dark regions on the sun's surface caused by magnetic activity. Analyzing sunspot data helps us understand solar cycles and predict solar phenomena. This project utilizes historical sunspot data to create predictive models for daily, monthly, and yearly sunspot activity using the Prophet time series forecasting library.

---

## Features

- Time series forecasting for three distinct intervals: **daily**, **monthly**, and **yearly**.
- Implements data preprocessing, model fitting, and evaluation.
- Evaluates model performance using metrics:
  - Mean Absolute Error (MAE)
  - Mean Absolute Percentage Error (MAPE)
  - R² Score
- Visualizations of forecasts and their components.

---

## Project Structure

```
├── Daily_Forecasting.ipynb   # Forecasting daily sunspot activity
├── Monthly_Forecasting.ipynb # Forecasting monthly sunspot activity
├── Yearly_Forecasting.ipynb  # Forecasting yearly sunspot activity
├── README.md                 # Project documentation
```

---

## Data Sources

The datasets used in this project are public sunspot data files in `.csv` format:

1. **Daily Data:** `SN_d_tot_V2.0.csv`
2. **Monthly Data:** `SN_m_tot_V2.0.csv`
3. **Yearly Data:** `SN_y_tot_V2.0.csv`

Each dataset includes:
- Date information.
- Sunspot counts.
- Additional statistical metadata.

---

## Requirements

Install the following Python packages to run the project:

```bash
pip install pandas matplotlib scikit-learn prophet
```

### Required Libraries
- `prophet`
- `pandas`
- `matplotlib`
- `scikit-learn`

---

## Usage

1. Clone the repository:
   ```bash
   git clone https://github.com/your-username/sunspot-forecasting.git
   cd sunspot-forecasting
   ```
2. Open and run each notebook in a Jupyter Notebook environment:
   - `Daily_Forecasting.ipynb`
   - `Monthly_Forecasting.ipynb`
   - `Yearly_Forecasting.ipynb`
3. Replace dataset paths with your local file paths if necessary.
4. Execute the cells to:
   - Preprocess data.
   - Train the Prophet model.
   - Visualize forecasts.
   - Evaluate model performance.

-----

#### Daily Model:
- **MAE:** *94.64854066599672*
- **MAPE:** *1.4163671597440288*
- **R²:** *1.4163671597440288*

#### Monthly Model:
- **MAE:** *53.3027443157509*
- **R²:** *0.06548493193477534*

#### Yearly Model:
- **MAE:** *2.928628759385342*
- **MAPE:** *0.5546846868302251*
- **R²:** *0.1810993217615129*

### Forecast Visualizations
Each notebook generates:
- Time series plots with predictions and confidence intervals.
- Trend component visualizations.

---

## Acknowledgements

- Data sourced from publicly available sunspot datasets.
- Inspired by Facebook's Prophet library.
