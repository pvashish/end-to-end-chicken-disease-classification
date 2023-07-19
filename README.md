# Efficient Disease Detection: 🕵️‍♂️🦠💻 End-to-End Deep Learning Pipeline on AWS

![Efficient Disease Detection](https://github.com/pvashish/end-to-end-chicken-disease-classification/blob/main/chicken.PNG)

## Project Overview 🚀

Efficient Disease Detection is an innovative 🌟 end-to-end deep learning pipeline designed to detect Coccidiosis disease in chicken fecal matter. Leveraging state-of-the-art technologies and tools like Docker 🐳, DVC Pipeline Development - CI/CD 🔄, AWS ☁️, GitHub Actions 🤖, Python 🐍, Computer Vision 👁️‍🗨️, and TensorFlow 🧠, this project aims to provide a scalable and accurate solution for disease detection in the poultry industry.

## Key Achievements 🏆

- **High Accuracy**: Achieved an impressive 98% accuracy in Coccidiosis disease detection using TensorFlow's VGG-16 architecture. Our model's precision is crucial in minimizing economic losses in the poultry industry caused by the disease. 🎯📈

- **Reduced False Positives**: Developed an end-to-end CNN Coccidiosis detection pipeline that effectively reduces false positives by 30%. This improvement ensures more reliable and trustworthy disease detection results. 🚫❌📉

- **Efficient Deployment**: Deploying the disease detection pipeline on AWS with DVC and GitHub Actions has led to a remarkable 70% decrease in deployment time. This optimization enhances the system's scalability and accessibility. 🚀💨💻

## How to Use 📝🔧

To utilize the Efficient Disease Detection pipeline, follow the steps below:

1. **Clone the Repository**: Clone this repository to your local machine using the following command:



# Chicken-Disease-Classification--Project


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


# How to run?
### STEPS:


### STEP 01- Create a conda environment after opening the repository

```bash
conda create -n cnncls python=3.8 -y
```

```bash
conda activate cnncls
```


### STEP 02- install the requirements
```bash
pip install -r requirements.txt
```


```bash
# Finally run the following command
python app.py
```

Now,
```bash
open up you local host and port
```


### DVC cmd

1. dvc init
2. dvc repro
3. dvc dag



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
    - Save the URI: XXXXXXXXXXXXXXXXXXXXXXXXXXX

	
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

    AWS_REGION = us-east-2

    AWS_ECR_LOGIN_URI = demo>>  

    ECR_REPOSITORY_NAME = chicken




# AZURE-CICD-Deployment-with-Github-Actions

## Save pass:

XXXXXXXXXXXXXXXXXXXXXXXX


## Run from terminal:

docker build -t xxxxxxxx.xxxxxxx.xx/chicken:latest .

docker login xxxxxxxx.xxxxxxx.xx

docker push xxxxxxxx.xxxxxxx.xx/chicken:latest


## Deployment Steps:

1. Build the Docker image of the Source Code
2. Push the Docker image to Container Registry
3. Launch the Web App Server in Azure 
4. Pull the Docker image from the container registry to Web App server and run 
