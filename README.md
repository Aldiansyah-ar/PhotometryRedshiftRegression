## Project Details: 
1. Team Members:
Aldiansyah Anugrah Ramadhan, Gia Muhammad Agusta, Giovaldi Ramadhan,  Muhammad Rizaldi Yani H.

2. Data Source: SDSS Data Release 18

3. Method:

```mermaid
graph TD;
    A[Start] --> B[Query Data from Database]
    B --> C[Data Preprocessing]
    C --> D[75% Train]
    C --> E[25% Test]

    D --> F1[Extra Tree Regressor]
    D --> F2[Random Forest]
    D --> F3[Deep Learning]

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

    K --> L[Output Model]
    L --> M[End]
```

Notes
* Data Preprocessing (filtering zWarning = 0, excluding the 'Star' class, handling outliers, filtering color index, train test split)
* Deep Learning (Deep Convolutional Neural Network)
* Hyperparameter Tuning (Random Search and Genetic Algorithm)
* Output Model (Redshift)

4. ML Category: Supervised Learning (Regression) 

5. Task Assignments: \\
a. Medium Story: Rizaldi and Gia \\
b. YouTube video: All members \\
c. Git code: Aldi \\
d. OSF Presentation slides: Giovaldi
