# End to End Text Summarizer Project 📚

## Workflows 🚀

1. 🛠️ Update `config.yaml` for project configurations.
2. ⚙️ Update `params.yaml` with necessary parameters.
3. 📖 Update entity details.
4. 📂 Update the configuration manager in the `src` config folder.
5. 🧩 Update the components.
6. 🔄 Update the pipeline.
7. 🚀 Update the `main.py` for project execution.
8. 📲 Update the `app.py` for user interface.

# How to Run? 🏃‍♀️

### STEPS:

👯‍♂️ Clone the repository


https://github.com/saibattula93/Text-summarization-project


📦 Create a conda environment after opening the repository


conda create -n summary python=3.8 -y



conda activate summary


🛠 Install the requirements


pip install -r requirements.txt


🚀 Finally, run the following command


python app.py


🌐 Now, open up your local host and port

👨‍💻 Author: Bappy Ahmed
📊 Data Scientist
✉️ Email: entbappy73@gmail.com

# AWS-CICD-Deployment-with-Github-Actions 🚢

## 1. Login to AWS console 🔑

## 2. Create IAM user for deployment 🤖

	# With specific access

	1. EC2 access: Virtual machine management.

	2. ECR: Elastic Container Registry to save your Docker images in AWS.

	# Description: About the deployment 🚀

	1. Build Docker image of the source code.

	2. Push your Docker image to ECR.

	3. Launch Your EC2.

	4. Pull Your image from ECR in EC2.

	5. Launch your Docker image in EC2.

	# Policy:

	1. AmazonEC2ContainerRegistryFullAccess

	2. AmazonEC2FullAccess

## 3. Create ECR repo to store/save Docker image

    - Save the URI: 566373416292.dkr.ecr.us-east-1.amazonaws.com/text-s

## 4. Create EC2 machine (Ubuntu) 🖥️

## 5. Open EC2 and Install Docker in EC2 Machine:

	# Optional

	sudo apt-get update -y

	sudo apt-get upgrade

	# Required

	curl -fsSL https://get.docker.com -o get-docker.sh

	sudo sh get-docker.sh

	sudo usermod -aG docker ubuntu

	newgrp docker

## 6. Configure EC2 as self-hosted runner:

    Setting > Actions > Runner > New Self-hosted Runner > Choose OS > Then run the command one by one

## 7. Setup GitHub secrets:

    AWS_ACCESS_KEY_ID=

    AWS_SECRET_ACCESS_KEY=

    AWS_REGION = us-east-1

    AWS_ECR_LOGIN_URI = demo >> 566373416292.dkr.ecr.ap-south-1.amazonaws.com

    ECR_REPOSITORY_NAME = simple-app 📦