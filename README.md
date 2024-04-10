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

## About MLflow & DVC
## MLflow

- Its Production Grade
- Trace all of your expriements
- Logging & taging your model

DVC

Its very lite weight for POC only
lite weight expriements tracker
It can perform Orchestration (Creating Pipelines)

## Data Version Control (DVC)

dvc init
dvc repro (to activate)
dvc dag ()

# AWS-CICD-Deployment-with-Github-Actions

## 1. Login to AWS console.

## 2. Create IAM user for deployment

	#with specific access

	1. EC2 access : It is virtual machine

	2. ECR: Elastic Container registry to save your docker image in aws


	#Description: About the deployment

	1. Build docker image of the source code

	2. Push your docker image to ECR

	3. Launch Your EC2 

	4. Pull Your image from ECR in EC2

	5. Lauch your docker image in EC2

	#Policy:

	1. AmazonEC2ContainerRegistryFullAccess

	2. AmazonEC2FullAccess

## 3. Create ECR repo to store/save docker image
    - Save the URI: 566373416292.dkr.ecr.us-east-1.amazonaws.com/chicken

	
## 4. Create EC2 machine (Ubuntu) 

## 5. Open EC2 and Install docker in EC2 Machine:
	
	
	#optinal

	sudo apt-get update -y

	sudo apt-get upgrade
	
	#required

	curl -fsSL https://get.docker.com -o get-docker.sh

	sudo sh get-docker.sh

	sudo usermod -aG docker ubuntu

	newgrp docker
	
# 6. Configure EC2 as self-hosted runner:
    setting>actions>runner>new self hosted runner> choose os> then run command one by one


# 7. Setup github secrets:

    AWS_ACCESS_KEY_ID=

    AWS_SECRET_ACCESS_KEY=

    AWS_REGION = us-east-1

    AWS_ECR_LOGIN_URI = demo>>  566373416292.dkr.ecr.ap-south-1.amazonaws.com

    ECR_REPOSITORY_NAME = simple-app


## run the the application

pip install flask
python app.py

# Note

remember to activate your venv everytime you start a new terminal .\vkidney\Scripts\activate
