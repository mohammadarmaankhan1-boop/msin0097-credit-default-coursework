# Credit Card Default Prediction

MSIN0097 Predictive Analytics Coursework

------------------------------------------------------------------------

## Repository Contents

-   credit_default_analysis_full_updated.ipynb → Main analysis notebook
-   Copy of default of credit card clients.xlsx → UCI dataset file
-   requirements.txt → pip environment specification
-   environment.yml → conda environment specification
-   README.md → Run and data instructions
-   .gitignore → Excludes temporary files

------------------------------------------------------------------------

## Project Overview

This project implements a binary classification model to predict whether
a customer will default on their credit card payment in the following
month.

The notebook includes:

-   Problem framing
-   Exploratory Data Analysis (EDA)
-   Data preprocessing
-   Model training and evaluation
-   Performance metrics suitable for imbalanced classification (ROC-AUC,
    Precision, Recall, F1)

------------------------------------------------------------------------

## Dataset Access Instructions

Source: Yeh, I.-C. (2009). Default of Credit Card Clients. UCI Machine
Learning Repository.

If submitting without the dataset due to licensing: 1. Visit the UCI
Machine Learning Repository. 2. Search for "Default of Credit Card
Clients". 3. Download the Excel file. 4. Place it in the SAME folder as
the notebook. 5. Ensure the file name matches exactly:

Copy of default of credit card clients.xlsx

The notebook loads the dataset using:

df = pd.read_excel("Copy of default of credit card clients.xlsx")

------------------------------------------------------------------------

## Installation

Python 3.11 recommended.

### Option 1 --- Conda

conda env create -f environment.yml conda activate credit-default
jupyter lab

### Option 2 --- pip

python -m venv .venv

Windows: .venv`\Scripts`{=tex}`\activate`{=tex}

macOS/Linux: source .venv/bin/activate

pip install -r requirements.txt jupyter lab

------------------------------------------------------------------------

## How to Run

Open the predictive assignment folder.

Ensure both files are present:

credit_default_analysis_full_updated.ipynb

Copy of default of credit card clients.xlsx

Launch Jupyter Lab from this folder.

Open the notebook and run all cells sequentially.

The dataset must remain in the same directory as the notebook to avoid file path errors.
------------------------------------------------------------------------

## Reproducibility

All required libraries are listed in requirements.txt and
environment.yml. No external APIs or additional dependencies are
required. Results should be reproducible if random seeds are fixed
within the notebook.

------------------------------------------------------------------------

## Troubleshooting

ModuleNotFoundError: → Ensure the correct environment is activated.

FileNotFoundError: → Confirm Copy of default of credit card clients.xlsx
is located in the same directory as the notebook.
