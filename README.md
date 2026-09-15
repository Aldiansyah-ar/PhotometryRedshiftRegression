# Photometric Redshift Estimation Using Regression
<p style="text-align: justify;">
  Redshift estimation using spectroscopic methods is constrained by high time consumption and computational costs. To overcome these limitations, a regression approach was implemented utilizing Extra Trees Regressor, Random Forest, and CNN algorithms. To optimize model performance, hyperparameter tuning was conducted using a genetic algorithm and random search.
</p>

## Data Collection
The SDSS data is gathered by SQL query on https://skyserver.sdss.org/dr18/SearchTools/sql

## Stack
Python (Scikitlearn, PyTorch)

## Setup

Clone the repository
```bash
git clone https://github.com/Aldiansyah-ar/PhotometryRedshiftRegression
```
Direct to the project directory
```bash
cd PhotometryRedshiftRegression
```
Create the `Python Environment`

```bash
python -m venv venv_name
```
Activate the environment
```bash
venv_name\scripts\activate.bat
```
Install the library in `requirements.txt`
```bash
pip install -r requirements.txt
```

## Project Member
- Aldiansyah Anugrah Ramadhan
- Muhammad Rizaldi Yani Hidayatulloh
- Gia Muhammad Agusta
- Giovaldi Ramadhan