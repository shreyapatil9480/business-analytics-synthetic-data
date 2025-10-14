## Business Analytics Synthetic Project

This repository contains a **synthetic business data project** designed to showcase
skills valuable for roles such as **business analyst**, **program manager** and
**data analyst**.  The project includes a synthetic dataset, a fully
documented Jupyter notebook with exploratory data visualisation and
predictive models, and a `requirements.txt` file listing the Python
dependencies.  Everything is organised so you can clone the repository and
run the analysis out of the box.

### Project structure

- **`data/synthetic_business_data.csv`** – A synthetically generated dataset
  representing two years of sales transactions.  Each row contains the
  transaction date, region, product category, marketing spend, units sold,
  revenue, customer satisfaction, and whether the customer churned.  The
  dataset was generated programmatically (see the notebook for details) and
  does not contain any real personal or proprietary information.

- **`analysis.ipynb`** – A Jupyter notebook that walks through the
  project in increasing levels of complexity:

  1. **Data loading & quality checks** – Introduce the dataset, inspect
     the shape and data types, handle missing values, and create a basic
     summary table.
  2. **Exploratory data visualisation** – Use charts such as bar plots,
     histograms, box plots and heatmaps to understand sales patterns
     across regions, products and time.  These visualisations help
     illustrate trends that are commonly investigated by business analysts
     and program managers.
  3. **Feature engineering & modelling** – Build predictive models using
     scikit‑learn.  The notebook demonstrates both regression (predicting
     revenue) and classification (predicting churn), including data
     splitting, training, evaluation metrics and interpretation of
     coefficients or feature importances.

- **`requirements.txt`** – Lists the Python libraries used in the project so you
  can install them in a fresh environment with `pip install -r
  requirements.txt`.  The dependencies include common data‑science
  packages such as pandas, numpy, seaborn, matplotlib, scikit‑learn and
  jupyter.

### Getting started

To reproduce the analysis on your machine:

1. **Clone the repository** and change into the directory:
   ```bash
   git clone <REPO-URL>
   cd <REPO-NAME>
   ```

2. **Create and activate a Python environment (optional but recommended):**
   ```bash
   python3 -m venv venv
   source venv/bin/activate
   ```

3. **Install dependencies:**
   ```bash
   pip install -r requirements.txt
   ```

4. **Launch Jupyter:**
   ```bash
   jupyter notebook analysis.ipynb
   ```

The notebook is organised with markdown explanations and commented code so
you can follow along, modify parameters, and explore the data further.

### Customisation and extensibility

This project provides a foundation that you can extend in several ways:

- **Add new features:**  Incorporate additional synthetic variables such as
  advertising channels, customer demographics or product prices.
- **Time‑series forecasting:**  Try ARIMA or prophet models to forecast
  future sales by product and region.
- **Dashboard creation:**  Use tools such as Plotly Dash or PowerBI to
  build an interactive dashboard summarising key insights.
- **Real data substitution:**  Swap the synthetic data with your own
  anonymised dataset to practise on information relevant to your target
  industry (e.g., finance, healthcare or retail).

### Licence

The code in this repository is provided under the MIT licence.  The
synthetic dataset is generated entirely by this project and may be used
without restriction.
