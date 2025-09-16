MLOps Assignment 1 – Experiment Tracking with MLflow 🧑‍💻

📌 Problem Statement

The objective of this assignment is to learn the basics of MLOps workflows, including:

Using GitHub for version control and reproducibility.

Training multiple ML models on a dataset.

Tracking experiments, metrics, and artifacts with MLflow.

Registering the best model in MLflow’s Model Registry.



📊 Dataset Description

I used the Iris dataset, a classic dataset for multi-class classification.

Samples: 150 (3 classes: Setosa, Versicolor, Virginica).

Features: 4 numeric features (sepal length, sepal width, petal length, petal width).

Target: Plant species (3 classes).

Reference: Scikit-learn Iris Dataset



⚙️ Model Training & Comparison

I trained 3 models using scikit-learn:

Logistic Regression

Random Forest Classifier

Support Vector Machine (SVM)



✅ Evaluation Metrics:
Accuracy

Weighted F1-score

Model	Accuracy	F1-score

Logistic Regression

Random Forest	

SVM	

👉 Best Model: Random Forest 🎉




📈 MLflow Tracking Results

Experiment results (parameters, metrics, confusion matrices) were logged using MLflow.

📸 Screenshot Example – MLflow Runs:

<img width="1539" height="837" alt="image" src="https://github.com/user-attachments/assets/4f8ea2c7-fcfe-480b-a8ef-c6671744b7c9" />


📸 Screenshot Example – Confusion Matrix Artifact:

<img width="698" height="578" alt="image" src="https://github.com/user-attachments/assets/7e7c7f5b-ba6f-470a-ad21-a12d56f7138f" />





🏆 Model Registration in MLflow

The best model (Random Forest) was registered in MLflow Model Registry under the name: iris-best-model.

Version: v1

Source: Run ID from best MLflow experiment

📸 Screenshot – Model Registry:

<img width="1569" height="906" alt="image" src="https://github.com/user-attachments/assets/163c3581-f613-4afc-8152-f40008dc9860" />





🚀 How to Run This Project

Step 1: Clone the Repository

git clone https://github.com/SaadAteeq-FOPSILHON/mlops-assignment-1.git

cd mlops-assignment-1


Step 2: Create Environment & Install Dependencies

pip install -r requirements.txt


Step 3: Run MLflow Tracking Server

mlflow ui


→ Open http://127.0.0.1:5000


Step 4: Run Training Notebook

jupyter notebook notebooks/model_training.ipynb

This will:

Train Logistic Regression, Random Forest, and SVM.

Log metrics, parameters, and artifacts to MLflow.

Save trained models inside /models.




📂 Project Structure

mlops-assignment-1/
├── data/               # (raw datasets, if any)
├── notebooks/          # Jupyter notebooks (training + MLflow)
│   └── model_training.ipynb
├── src/                # (helper scripts if extended later)
├── models/             # saved trained models (.pkl)
├── results/            # plots, confusion matrices, screenshots
├── README.md           # project documentation
├── requirements.txt    # package dependencies




