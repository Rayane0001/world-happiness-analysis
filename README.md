# 🌍 World Happiness Analysis

> **Comprehensive data science project exploring global happiness factors through statistical analysis and interactive visualizations.**

[![Python](https://img.shields.io/badge/Python-3.x-3776AB?logo=python&logoColor=white)](https://python.org/)
[![Jupyter](https://img.shields.io/badge/Jupyter-Notebook-F37626?logo=jupyter&logoColor=white)](https://jupyter.org/)
[![Pandas](https://img.shields.io/badge/Pandas-Latest-150458?logo=pandas&logoColor=white)](https://pandas.pydata.org/)

## 👥 Authors

- **Rayane Rousseau** - Lead Data Scientist, Statistical Analysis & Visualization
- **Gibril Zaoui** - Verification, Oral Presentation Support & General Assistance

---

## 🚀 Quick Start

```bash
# Clone the repository
git clone https://github.com/Rayane0001/world-happiness-analysis
cd world-happiness-analysis

# Install dependencies
pip install pandas numpy matplotlib seaborn statsmodels plotly openpyxl xlrd

# Open the notebook
jupyter notebook happiness_analysis.ipynb
```

---

## 🎯 Project Overview

This project explores the factors that influence happiness across the world. Using Python and multiple datasets (primarily from Kaggle), we analyze how elements like economy, society, health, governance, and environment relate to population well-being.

All analyses and visualizations are presented in the Jupyter notebook `happiness_analysis.ipynb`.

---

## 📊 Research Questions

We explore 15 comprehensive analytical questions:

1. **Relative Impact of Factors on Happiness**
2. **Economic Outlier Countries**
3. **Regional Happiness Disparities**
4. **Freedom and Well-being by Context**
5. **Government Trust and Corruption**
6. **Generosity and Economic Resilience**
7. **Unexplained Residual Analysis (Dystopia Residual)**
8. **Social Support and Regional Well-being**
9. **Freedom-Corruption Interaction on Happiness**
10. **Temporal Evolution of Happiness Factors**
11. **Evaluative vs. Emotional Happiness by Region**
12. **Gender Inequality, HDI, and Happiness**
13. **Specific Health Metrics and Happiness (GDP-Controlled)**
14. **Sustainable Development - Happiness, Development & Ecological Footprint**
15. **Governance Profiles - Objective Freedom and Corruption Interaction**

### General Conclusion
A **happiness map** was created to visualize the best countries to live in, concluding by considering all studied criteria.

---

## 📁 Project Structure

```
.
├── happiness_analysis.ipynb  # Jupyter notebook with analyses
├── CSVs/                     # Datasets used (Source: Kaggle)
│   ├── civil_liberties_score_fh_new.csv
│   ├── CPI2023_global_results_trends.csv
│   ├── hdr_general.csv
│   ├── world_happiness_report_2024.csv
│   └── world_population_and_health.csv
├── .gitignore
├── LICENSE
└── README.md
```

---

## 📦 Datasets (`CSVs/`)

Five primary datasets downloaded from [Kaggle](https://www.kaggle.com/) (combining data from World Happiness Report, UNDP, World Bank, Freedom House, Transparency International):

1. **`world_happiness_report_2024.csv`** - Central happiness scores (Life Ladder) with 6 key factors (GDP per capita, social support, life expectancy, freedom, generosity, corruption)
2. **`hdr_general.csv`** - Human Development Index (HDI), gender inequality, education, environmental indicators (CO2)
3. **`CPI2023_global_results_trends.csv`** - Corruption Perception Index 2023 with regional classification
4. **`civil_liberties_score_fh_new.csv`** - Civil liberties scores (Freedom House)
5. **`world_population_and_health.csv`** - Population and specific health indicators (infant mortality, malnutrition)

---

## 🛠️ Tech Stack

### Core Libraries
- **Pandas** - Data manipulation and cleaning
- **NumPy** - Numerical computations
- **Matplotlib** - Base plotting and figure creation
- **Seaborn** - Statistical visualizations

### Statistical Analysis
- **Statsmodels** - Linear regression (OLS), interaction models, partial regression plots

### Interactive Visualization
- **Plotly** - Interactive choropleth maps and dynamic charts

### Data Processing
- **OpenPyXL** - Excel file handling
- **XLRD** - Legacy Excel format support

---

## 💡 Key Features

📈 **Statistical Modeling** - OLS regression with interaction terms  
🗺️ **Interactive Maps** - Plotly choropleth visualizations  
📊 **Comprehensive Visualizations** - Heatmaps, regression plots, faceted charts  
🔍 **Multi-dimensional Analysis** - Economic, social, health, governance factors  
🌱 **Sustainability Assessment** - Happiness vs. ecological footprint  
📉 **Temporal Analysis** - Evolution of happiness factors over time  

---

## 📈 Key Findings

**Happiness isn't just about money!** Strong social connections, sense of freedom, good health, low corruption, and equality are equally or more important.

The world faces significant happiness inequality, and balancing high well-being with environmental respect remains a major challenge.

Countries that perform best typically combine:
- **Economic performance**
- **Social cohesion**
- **Good governance**

---

## 🎓 Analysis Techniques

- **Correlation Analysis** - Identifying relationships between variables
- **Linear Regression** - OLS models with interaction terms
- **Statistical Testing** - P-values, R², coefficient significance
- **Partial Regression** - Controlling for confounding variables
- **Categorical Analysis** - Regional and governance profile comparisons
- **Time Series** - Temporal evolution patterns
- **Geospatial Visualization** - Interactive world maps

---

## 📝 Usage

1. Place CSV files in the `CSVs/` subfolder
2. Open `happiness_analysis.ipynb` with **JupyterLab, Jupyter Notebook, VS Code, PyCharm** or any compatible IDE
3. Execute cells in order to obtain analyses, visualizations, and detailed interpretations

---

## 🔬 Research Highlights

✅ **Comprehensive Data Integration** - 5 major international datasets  
✅ **Advanced Statistical Methods** - Regression modeling with interactions  
✅ **Interactive Visualizations** - Dynamic choropleth maps  
✅ **Multi-factor Analysis** - Economic, social, health, governance dimensions  
✅ **Sustainability Focus** - Environmental impact considerations  
✅ **Regional Comparisons** - Cross-cultural happiness patterns  

---

<div align="center">

**Understanding global happiness through data science** 🌏

[⭐ Star this repository](https://github.com/Rayane0001/world-happiness-analysis)

</div>
