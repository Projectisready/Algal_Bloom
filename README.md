# Algal Bloom Analysis: Environmental Drivers of Cyanobacteria in U.S. Lakes

## Project Overview

This project investigates environmental factors associated with cyanobacteria abundance in lakes across the conterminous United States.

The analysis uses data published by the U.S. Environmental Protection Agency (EPA), containing lake observations together with water-quality, watershed, land-use, climate, and other environmental variables.

The project is organised into two main parts:

### Part 1 — Exploratory Data Analysis (EDA)

The first part explores the characteristics of the dataset and investigates relationships between cyanobacteria abundance and selected environmental variables.

The main variables examined are:

- `B_G_DENS` — Cyanobacteria cell abundance (cells/mL)
- `TEMPERATURE` — Water temperature (°C)
- `PTL` — Total phosphorus concentration (mg/L)
- `NTL` — Total nitrogen concentration (mg/L)
- `CHLA_RESULT` — Chlorophyll-a concentration (mg/L)

The EDA includes:

- Dataset inspection and descriptive statistics
- Missing-value analysis
- Distribution analysis
- Log transformation of highly skewed variables
- Pearson correlation analysis
- Spearman rank correlation analysis
- Scatter plots and regression-line visualisations

Initial exploratory results indicate positive associations between cyanobacteria abundance and the selected environmental variables. Chlorophyll-a showed the strongest association, followed by total nitrogen and total phosphorus, while water temperature showed a weaker positive association.

These findings represent statistical associations and should not be interpreted as evidence of causation.

### Part 2 — Regression Modelling

The second part of the project will extend the exploratory analysis by developing regression models to investigate and predict cyanobacteria abundance using environmental variables.

Planned work includes:

- Selection of predictor variables
- Assessment of multicollinearity
- Development of regression models
- Model diagnostics and assumption checking
- Training and testing/validation
- Evaluation using appropriate regression performance metrics
- Interpretation and comparison of model results

Part 2 will be developed after completion of the exploratory analysis.

## Dataset

The project uses the EPA dataset:

**Dataset: Predictions of Cyanobacteria and Microcystin in Lakes across the Conterminous United States**

The main files used in this project are:

- `HABsDrivers_Model_Data.csv`
- `HABsDrivers_Model_Metadata.csv`

The model dataset contains National Lakes Assessment observations combined with environmental variables used to investigate potential drivers of harmful algal blooms.

### Data Source

U.S. Environmental Protection Agency (EPA)

Dataset DOI: **10.23719/1532353**

EPA dataset page:
https://assessments.epa.gov/risk/document/%26deid%3D366355

Data.gov catalogue:
https://catalog.data.gov/dataset/dataset-predictions-of-cyanobacteria-and-microcystin-in-lakes-across-the-conterminous-unit

## Dataset Citation

Handler, A., Reynolds, M., Compton, J., Dumelle, M., Weber, M., Jansen, L., Hill, R., Brehob, M., Sabo, R., & Pennino, M. (2025). *Dataset: Predictions of Cyanobacteria and Microcystin in Lakes across the Conterminous United States.* U.S. Environmental Protection Agency, Washington, DC. DOI: 10.23719/1532353.

## Tools and Technologies

- Python
- Pandas
- NumPy
- Matplotlib
- Seaborn
- Jupyter Notebook
- Conda

## Project Structure

```text
algal-bloom-analysis/
│
├── README.md
├── data/
│   ├── HABsDrivers_Model_Data.csv
│   └── HABsDrivers_Model_Metadata.csv
│
├── notebooks/
│   ├── 01_exploratory_analysis.ipynb
│   └── 02_regression_analysis.ipynb    # Future work
│
└── figures/