# Airline Loyalty Program Analysis ✈️
This project consists of an exploratory data analysis of an airline loyalty program dataset, completed as part of a Data Analysis bootcamp module evaluation. It covers data cleaning and merging, statistical analysis, data visualization, and an evaluation of flight booking differences by education level.

## Tech Stack 🔧
Python 3.14.3 · Jupyter Notebook

**Libraries used:**
* `pandas` — data manipulation and DataFrame management
* `numpy` — numerical operations
* `seaborn` — statistical data visualization
* `matplotlib` — plot rendering and figure customization
* `sklearn` — advanced missing value imputation (IterativeImputer)

---

## Project Structure 🧬

```
src/
├── data/
│   ├── Customer Flight Activity.csv        — Raw flight activity dataset
│   ├── Customer Loyalty History.csv        — Raw customer profile dataset
│   └── Customer_Flight_Loyalty_Clean.csv   — Merged and cleaned dataset
├── figures/
│   ├── 02_Statistical_Analysis_Figures/    — Figures generated in Phase 2
│   └── 03_Visualisation_figures/           — Figures generated in Phase 3
└── notebooks/
├── 01_EDA_Merge_and_Cleaning.ipynb     — Phase 1: EDA, merging and data cleaning
├── 02_Statistical_Analysis.ipynb       — Phase 2: Statistical analysis and descriptive insights
└── 03_Visualisation_and_Flight_Booking_Differences_by_Education_Level.ipynb — Phase 3 & 4: Visualisation and education-level analysis
```
---

## Project Overview 🔩

**Phase 1 — EDA, Merge and Cleaning**
* Exploratory analysis of two independent datasets (flight activity and customer profiles)
* Dataset merging via left join on `Loyalty Number`
* Data cleaning: duplicate removal, null value treatment via IterativeImputer, type validation and logical consistency checks
* Export of the cleaned dataset for use in subsequent phases

**Phase 2 — Statistical Analysis**
* Descriptive statistics (mean, median, mode, standard deviation) for relevant numerical variables
* Outlier detection using the IQR method, supported by boxplot visualization
* Spearman correlation analysis with heatmap and scatterplot illustrations
* Frequency distribution analysis for relevant categorical variables

**Phase 3 — Visualisation**
* Monthly flight booking distribution (line plot by year)
* Distance vs. points accumulated correlation (scatter plot)
* Customer distribution by province (bar plot)
* Average salary by education level (box plot)
* Loyalty card tier proportion (pie chart)
* Customer distribution by marital status and gender (grouped bar plot)

**Phase 4 — Flight Booking Differences by Education Level**
* Filtered dataset to `Flights Booked` and `Education` columns
* Descriptive statistics per education group (mean and standard deviation)
* Conclusion: education level does not significantly influence flight booking volume

---
## Getting Started ▶️

### 1. Clone the repository
```
git clone https://github.com/Adalab/bda-modulo-3-evaluacion-final-MATC-90.git
```

### 2. Install the required libraries
```
pip install pandas numpy seaborn matplotlib scikit-learn
```

### 3. Run the notebooks in order
Open the notebooks in the `src/notebooks/` folder and execute them sequentially, starting with `01_EDA_Merge_and_Cleaning.ipynb`.

