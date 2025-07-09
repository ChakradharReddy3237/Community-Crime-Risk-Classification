# Community Crime Risk Classification with Objective-Driven Optimization

![Language](https://img.shields.io/badge/Language-Python-blue.svg)
![License](https://img.shields.io/badge/License-MIT-green.svg)

This repository contains the code, dataset, and final research paper for a machine learning project focused on predicting community crime risk levels. The project implements a dual-model framework to separately classify violent and non-violent crime, optimizing for a real-world public safety objective rather than generic accuracy.

---

## 📖 Project Overview

This study presents a comprehensive machine learning framework for classifying community crime levels by strategically distinguishing between violent and non-violent offenses. Utilizing the "Communities and Crime" dataset, a dual-model architecture is implemented to separately predict risk categories, validating the hypothesis that their socio-economic drivers are distinct.

The project's primary contribution is its **objective-driven optimization**. Instead of maximizing simple accuracy, the models were tuned to maximize **recall for the "high-risk" category**. This approach is critical in a public safety context, as the cost of a false negative (failing to identify a high-risk community) is substantially higher than that of a false positive.

The final models serve as powerful, practical tools for data-driven policy-making and resource allocation, achieving exceptional performance in identifying at-risk communities.

### ✨ Key Features

-   **Dual-Model Architecture:** Uses separate, specialized models (**XGBoost** for violent crime, **LightGBM** for non-violent crime) to capture the unique drivers of each crime type.
-   **Objective-Driven Tuning:** The entire optimization pipeline prioritizes maximizing recall for the high-risk class, achieving **99% recall for violent crime** and **94% recall for non-violent crime**.
-   **Advanced Feature Selection:** Employs Recursive Feature Elimination with Cross-Validation (RFECV) to identify the most impactful socio-economic predictors for each model.
-   **Comprehensive Analysis:** The entire workflow, from data imputation and feature engineering to model validation, is documented in the accompanying Jupyter Notebook and research paper.

---

## 📂 Repository Structure

```
├── A Dual-Model Framework....pdf   # The complete research paper with detailed methodology and findings.
├── Community-Crime-Risk-Classification.ipynb   # The main Jupyter Notebook with all the Python code.
├── crime_dataset.csv             # The raw dataset used for the project.
├── requirements.txt              # A list of Python libraries required to run the notebook.
└── README.md                     # You are here!
```

---

## ⚙️ Technologies Used

-   **Language:** Python 3
-   **Libraries:**
    -   Pandas & NumPy (Data Manipulation)
    -   Scikit-learn (Preprocessing, Modeling, RFECV)
    -   XGBoost & LightGBM (Gradient Boosting Models)
    -   Matplotlib & Seaborn (Data Visualization)
    -   Jupyter Notebook (Code Environment)

---

## 🚀 How to Run

To run this project on your local machine, follow these steps:

1.  **Clone the repository:**
    ```bash
    git clone https://github.com/ChakradharReddy3237/Community-Crime-Risk-Classification.git
    cd Community-Crime-Risk-Classification
    ```

2.  **Create a virtual environment (recommended):**
    ```bash
    python -m venv venv
    source venv/bin/activate  # On Windows, use `venv\Scripts\activate`
    ```

3.  **Install the required libraries:**
    ```bash
    pip install -r requirements.txt
    ```

4.  **Launch Jupyter Notebook:**
    ```bash
    jupyter notebook
    ```

5.  Open the `Community-Crime-Risk-Classification.ipynb` file and run the cells.

---

## License

