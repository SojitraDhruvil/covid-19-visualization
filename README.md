# COVID-19 Data Exploration & Statistical Analysis 📊

A comprehensive data science repository analyzing COVID-19 trends, spatial distribution, and statistical metrics at both the National (India) and Global levels.

---

## 📂 Repository Reorganization Layout

The repository is organized cleanly into separate folders for **India** and **World** datasets and notebooks:

```text
covid-19-visualization/
├── india/
│   ├── Latest Covid-19 India Status.csv               # India dataset
│   ├── covid-19-india-eda-visualization-report.ipynb # India analysis notebook
│   ├── images/
│   │   ├── india_covid_cover.png                       # India report cover
│   │   └── india New Cases Calendar Heatmap.png
│   └── iframe_figures/                                 # Plotly offline HTML exports
│
├── world/
│   ├── covid19_clean_data.csv                          # Cleaned global cases
│   ├── time_series_covid19_confirmed_global.csv       # Global time-series cases
│   ├── time_series_covid19_deaths_global.csv          # Global time-series deaths
│   ├── merged_uncleaned_data.csv
│   ├── Covid-19 EDA and Visualization.ipynb           # Consolidated Global notebook
│   └── images/
│       ├── world_covid_cover.png                       # World report cover
│       ├── Global COVID-19 Trend.png
│       ├── Heat Map Confirmed Cases.png
│       ├── Heat Map Deaths.png
│       └── US New Cases Calendar Heatmap.png
│
├── .gitignore                                          # Excludes generated html assets
└── requirements.txt                                    # Python dependencies list
```

---

## 📓 Notebook Overview

### 🇮🇳 1. India COVID-19 Report
* **Path**: `india/covid-19-india-eda-visualization-report.ipynb`
* **Focus**: State-wise analysis of confirmed cases, recovery (discharge) ratios, active infection rates, and mortality indicators in India.
* **Key Visuals**: Choropleth maps of India showing case concentrations, recovery-to-active correlations, state-by-state comparisons, and mortality patterns.

### 🌐 2. Global COVID-19 Report & Statistical Testing
* **Path**: `world/Covid-19 EDA and Visualization.ipynb`
* **Focus**: Consolidated analysis of international COVID-19 progression, combining interactive timelines, geographical mapping, country comparison curves, and rigorous statistical tests.
* **Key Analysis & Tests**:
  * **Exploratory Data Analysis**: Top 10 worst-affected countries, global rolling averages of daily infections, and mortality rate distribution.
  * **Hypothesis Testing**: Two-sample t-test comparing India's case-fatality rate against the top 10 highest fatality rate nations.
  * **Correlation & Chi-Square Independence Tests**: Determining structural dependencies between cases and deaths.
  * **Linear Regression**: Assessing statistical dependencies between overall fatality rates and population volumes.

---

## 🛠️ Setup & Execution

### 1. Prerequisites
Ensure you have **Python 3.9+** installed on your system.

### 2. Install Dependencies
Install all the required Python libraries using `pip`:
```bash
pip install -r requirements.txt
```

### 3. Run the Jupyter Notebooks
Open the notebooks using Jupyter Notebook, JupyterLab, or VS Code:
```bash
jupyter notebook
```
> **Note**: Plotly charts are configured to render offline via `iframe` or `notebook_connected` modes to ensure high compatibility inside Jupyter notebook viewers without requiring browser redirects.
