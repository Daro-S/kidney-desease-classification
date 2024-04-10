# Kidney Disease Classification Project

Dataset: `https://www.kaggle.com/datasets/nazmul0087/ct-kidney-dataset-normal-cyst-tumor-and-stone`

## Workflows

1. Update config.yaml
2. Update secrets.yaml [Optional]
3. Update params.yaml
4. Update the entity
5. Update the configuration manager in src config
6. Update the components
7. Update the pipeline
8. Update the main.py
9. Update the dvc.yaml
10. app.py

## Project Description

This project aims to classify kidney disease based on various health metrics.

## Installation

To set up a local development environment:

1. Clone the repository: `git clone https://github.com/Daro-S/kidney-desease-classification.git`
2. Navigate into the cloned project: `cd kidney-desease-classification`
3. Create a virtual environment: `python -m venv vkidney`
4. Activate the virtual environment: `.\vkidney\Scripts\activate`
5. Install the dependencies: `pip install -r requirements.txt`

## Mlflow UI

## Dagshub remote server

Run this to export as env variables:

export MLFLOW_TRACKING_URI=https://dagshub.com/darosim.itdev/kidney-desease-classification.mlflow

export MLFLOW_TRACKING_USERNAME=darosim.itdev

export MLFLOW_TRACKING_PASSWORD=c63426cbd6f6a12861a78c26d0cb97a9235a1150

## Data Version Control (DVC)

dvc init
dvc repro (to activate)
