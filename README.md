Customer Churn Prediction — Deep Learning (Keras)

A complete end-to-end project performing customer churn prediction using data preprocessing, visualization, and deep learning models built with Keras.
This project is part of the Artificial Intelligence Certification Course and demonstrates real-world telecom churn analysis.

🚀 Project Overview

Telecom company Leo is experiencing customer churn and wants to identify at-risk customers using predictive analytics.
This project:

✔ Preprocesses and analyzes the churn dataset
✔ Performs feature engineering and exploratory data analysis (EDA)
✔ Builds three Keras neural network models
✔ Compares their performance
✔ Generates visualizations and a full project report
Customer-Churn-Analysis/
│
├── data/
│   └── customer_churn.csv          # (Upload your dataset here)
│
├── notebooks/
│   └── Churn_Analysis.ipynb        # Jupyter Notebook (to be generated)
│
├── reports/
│   └── customer_churn_project_report.pdf   # Auto-generated PDF report
│
├── src/
│   ├── preprocessing.py
│   ├── visualization.py
│   ├── model_1.py                  # tenure → churn
│   ├── model_2_dropout.py
│   └── model_3_multi_feature.py
│
└── README.md                       # This file
Tasks Performed
A) Data Manipulation

Count male customers

Count DSL internet customers

Extract female senior citizens paying via Mailed check

Extract customers with:

tenure < 10 months

OR total charges < $500

B) Data Visualization

Pie chart: Churn distribution

Bar plot: Internet service categories (DSL, Fiber, None)

🔥 C) Deep Learning Models (Keras)
Model 1 — Base Model

Feature: tenure

Layers:

Input: 12 neurons, ReLU

Hidden: 8 neurons, ReLU

Output: Sigmoid

Optimizer: Adam

Epochs: 150

Outputs:

Confusion matrix

Accuracy vs Epochs plot

Model 2 — With Dropout Regularization

Same as Model 1, plus:

Dropout (0.3) after input

Dropout (0.2) after hidden layer

Trained for 150 epochs

Model 3 — Multi-Feature Model

Features:

tenure

Monthly Charges

Total Charges

Layers:

Input: 12 neurons (dim = 3)

Hidden: 8 neurons

Output: Sigmoid

Outputs:

Confusion matrix

Accuracy plot

🧠 Technologies Used

Python

Pandas, NumPy

Matplotlib, Seaborn

TensorFlow / Keras

Scikit-Learn

📄 Generated Outputs

This project automatically generates:

📌 PDF Report
📌 All visualizations (PNG)
📌 Trained Models (.h5)
📌 Complete Jupyter Notebook (.ipynb)

▶️ How to Run

Place dataset in /data/customer_churn.csv

Open and run Churn_Analysis.ipynb

View outputs in /reports/

To generate fresh reports using ChatGPT:
Upload the dataset & request: "Run churn analysis"

🎯 Conclusion

This project provides a production-ready churn prediction workflow and demonstrates practical deep learning for business analytics.
