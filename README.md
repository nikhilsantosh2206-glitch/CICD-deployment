# CICD-deployment

## Project Overview

CICD-deployment is a Machine Learning project that demonstrates the implementation of a CI/CD pipeline using GitHub Actions. The project trains and evaluates a machine learning model on the Iris dataset and automatically executes the workflow whenever code changes are pushed to the repository.

## Features

* Automated Machine Learning model training
* Iris dataset classification
* Performance evaluation and metrics generation
* Confusion Matrix visualization
* Feature Importance analysis
* GitHub Actions CI/CD integration
* Automated artifact generation

## Tech Stack

* Python 3.11
* NumPy
* Pandas
* Scikit-Learn
* Matplotlib
* Seaborn
* GitHub Actions

## Project Structure

```text
CICD-deployment/
│
├── .github/
│   └── workflows/
│       └── cicd.yaml
│
├── iris.csv
├── train_model.py
├── test.py
├── requirements.txt
├── scores.txt
├── ConfusionMatrix.png
├── FeatureImportance.png
└── README.md
```

## Installation

Clone the repository:

```bash
git clone https://github.com/<your-username>/CICD-deployment.git
cd CICD-deployment
```

Install dependencies:

```bash
pip install -r requirements.txt
```

## Run the Training Pipeline

```bash
python train_model.py
```

## Outputs

The pipeline generates:

* `scores.txt` – Model evaluation metrics
* `ConfusionMatrix.png` – Confusion matrix visualization
* `FeatureImportance.png` – Feature importance visualization

## CI/CD Workflow

The GitHub Actions workflow automatically:

1. Checks out the repository
2. Sets up Python
3. Installs dependencies
4. Trains the model
5. Generates evaluation reports
6. Uploads generated artifacts

## Future Improvements

* Model versioning with MLflow
* Docker containerization
* Deployment using Flask/FastAPI
* Cloud deployment (AWS/Azure/GCP)
* MLOps integration
