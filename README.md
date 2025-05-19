# Solar Challenge Week 1

This repository contains the setup and analysis for Week 1 of the Solar Challenge project, including environment configuration, exploratory data analysis (EDA), and cross-country solar data comparison.

---

##  Environment Setup

Follow the steps below to reproduce the environment:

### 1. Clone the repository
```bash
git clone https://github.com/YOUR_USERNAME/solar-challenge-week1.git
cd solar-challenge-week1
```
### 2. Create and activate a virtual environment
```bash
python3 -m venv venv
source venv/bin/activate  # Windows: venv\Scripts\activate
```
### 3. Install dependencies
```bash
pip install -r requirements.txt
```
### 4. Folder Structure
```bash

├── .github/
│   └── workflows/
│       └── ci.yml
│       └── unittests.yml
├── .vscode/
│   └── settings.json
├── notebooks/
│   ├── README.md
│   └── __init__.py
│   └── benin_eda.ipynb
│   └── compare_countries.ipynb
│   └── sierraleone_eda.ipynb
│   └── togo_eda.ipynb
└── scripts/
│   ├── __init__.py
│   └── README.md
├── tests/
│   └── __init__.py
├── .gitignore
├── README.md
├── requirements.txt

```

---

## Exploratory Data Analysis (EDA)

Each country has its own EDA notebook under `notebooks/`.

To perform EDA for a country:

1. Create a new branch:
   ```bash
   git checkout -b eda-<country>
    ```

2. Create a new notebook named `<country>_eda.ipynb` inside the `notebooks/` folder.

3. Follow the EDA checklist:

   * Summary statistics and missing values
   * Outlier detection
   * Cleaning and exporting to `data/<country>_clean.csv`
   * Visual analysis of time series, wind, temperature, and solar irradiance
   * Correlation heatmaps, scatter plots, and bubble charts

4. Export cleaned CSV files to the `data/` folder.


---

## Project Implementation

The following tasks were completed as part of Week 1:

* **Task 1:** GitHub repository setup with virtual environment and CI workflow.

  * Created `.gitignore`, `requirements.txt`, and `.github/workflows/ci.yml`
  * Verified setup using GitHub Actions
* **Task 2:** Performed data profiling, cleaning, and EDA for individual countries.

  * EDA included missing value analysis, outlier removal, and visualization
* **Task 3:** Cross-country comparison using combined cleaned datasets

  * Visual comparison of GHI, DNI, DHI using boxplots and bar charts
  * Statistical testing using ANOVA and Kruskal-Wallis to assess significance
  * Key insights were summarized in markdown format

---

## Contributions

This work was completed individually as part of the Solar Challenge project.

* Set up GitHub repository with clean folder structure and CI pipeline
* Performed end-to-end EDA for the Benin dataset
* Developed `compare_countries.ipynb` to compare solar metrics across Benin, Sierra Leone, and Togo
* Implemented boxplots, summary tables, and statistical testing with p-value interpretation
* Documented key findings and added project-level documentation (this README and reports)

---


## ⚠️ Note About `data/` Folder

The `data/` folder is listed in `.gitignore` and should **not be committed** to version control.

Any CSV outputs (e.g., cleaned datasets) should go in `data/`, but **should not be added with `git add`**.

This helps keep the repository clean and avoids committing large files.




