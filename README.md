# Solar Challenge Week 1

This repository contains the setup for Week 1 of the Solar Challenge project, including environment configuration and CI integration using GitHub Actions.

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
├── .vscode/
│   └── settings.json
├── .github/
│   └── workflows/
│       └── ci.yml
│       └── unittests.yml
├── .gitignore
├── requirements.txt
├── README.md
├── src/
├── notebooks/
│   ├── __init__.py
│   └── README.md
├── tests/
│   └── __init__.py
└── scripts/
    ├── __init__.py
    └── README.md
```

## 📊 Exploratory Data Analysis (EDA)

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



## ⚠️ Note About `data/` Folder

The `data/` folder is listed in `.gitignore` and should **not be committed** to version control.

Any CSV outputs (e.g., cleaned datasets) should go in `data/`, but **should not be added with `git add`**.

This helps keep the repository clean and avoids committing large files.




