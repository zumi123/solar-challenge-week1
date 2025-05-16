# Solar Challenge Week 1

This repository contains the setup for Week 1 of the Solar Challenge project, including environment configuration and CI integration using GitHub Actions.

##  Environment Setup

Follow the steps below to reproduce the environment:

### 1. Clone the repository
```bash
git clone https://github.com/YOUR_USERNAME/solar-challenge-week1.git
cd solar-challenge-week1

### 2. Create and activate a virtual environment

python3 -m venv venv
source venv/bin/activate  # Windows: venv\Scripts\activate

### 3. Install dependencies
pip install -r requirements.txt

### ├── .vscode/
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

