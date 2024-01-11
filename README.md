# mlflowProject

Implemented a wine quality prediction project using MLOps and MLflow. Utilized the Wine Quality dataset, developed machine learning models, and deployed them on an EC2 instance. This project aimed to gain hands-on experience in MLOps principles and the effective use of MLflow for model tracking and deployment.

## Workflows

1. Update config.yaml
2. Update schema.yaml
3. Update params.yaml
4. Update the entity
5. Update the configuration manager in src config
6. Update the components
7. Update the pipeline 
8. Update the main.py
9. Update the app.py


# How to run?
### STEPS:

Clone the repository

```bash
https://github.com/manisha-v/mlflowProject.git
```

Install the requirements
```bash
pip install -r requirements.txt
```

Run the project
```bash
python app.py
```

Now,
```bash
open up you local host and port
```


### dagshub
[dagshub](https://dagshub.com/)

MLFLOW_TRACKING_URI=https://dagshub.com/manisha-v/mlflowProject.mlflow \
MLFLOW_TRACKING_USERNAME=manisha-v \
MLFLOW_TRACKING_PASSWORD=your-token  \
python script.py

Run this to export as env variables:

```bash

export MLFLOW_TRACKING_URI=https://dagshub.com/manisha-v/mlflowProject.mlflow

export MLFLOW_TRACKING_USERNAME=manisha-v

export MLFLOW_TRACKING_PASSWORD=your-token

```



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
    - Save the URI

	
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

    AWS_ECR_LOGIN_URI = 

    ECR_REPOSITORY_NAME = 

Commit the code and enjoy!

## Need any help?
##### Connect me on [LinkedIn](https://www.linkedin.com/in/manisha-varshney-914646191/)  <img src="https://cdn.iconscout.com/icon/free/png-256/linkedin-162-498418.png" width="25"> 


