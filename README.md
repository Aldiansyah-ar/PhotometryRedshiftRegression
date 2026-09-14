# Photometric Redshift Estimation Using Regression

<p style="text-align: justify;">
  Redshift estimation using spectroscopic methods is constrained by high time consumption and computational costs. To overcome these limitations, a regression approach was implemented utilizing Extra Trees Regressor, Random Forest, and CNN algorithms. To optimize model performance, hyperparameter tuning was conducted using a genetic algorithm and random search.
</p>

## Data Collection

* The SDSS data is gathered by SQL query on https://skyserver.sdss.org/dr18/SearchTools/sql

## Stack

Python (Scikitlearn, PyTorch)

## Methods

```mermaid
graph TD;
    A[Start] --> B[Query Data from Database]
    B --> C[Data Preprocessing]
    C --> D[75% Train]
    C --> E[25% Test]

    D --> F1[Extra Tree Regressor]
    D --> F2[Random Forest]
    D --> F3[CNN]

    F1 --> G1["Evaluate (R2, MAE, MSE)"]
    F2 --> G2["Evaluate (R2, MAE, MSE)"]
    F3 --> G3["Evaluate (R2, MAE, MSE)"]

    G1 --> H[Final Model]
    G2 --> H
    G3 --> H

    H --> I["Hyperparameter Tuning"]
    I --> J["Evaluate (R2, MAE, MSE)"]
    J --> K[Test Model]
    E --> K

    K --> L[Redshift]
    L --> M[End]
```

## Project Member
- Aldiansyah Anugrah Ramadhan
- Muhammad Rizaldi Yani Hidayatulloh
- Gia Muhammad Agusta
- Giovaldi Ramadhan
