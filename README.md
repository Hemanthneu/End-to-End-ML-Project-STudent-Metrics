**🔍End-to-End Production Grade ML Project**

**Student Performance Prediction for Machine Learning Model**
![Logo]([https://example.com/images/logo.png](https://github.com/Hemanthneu/End-to-End-ML-Project-Student-Metrics/blob/master/MLOps%20Process.png)

This project adopts a modular coding approach, leveraging various technologies to build an end-to-end solution. The primary technologies used in this project include:

**🐍 Python:** Python, a versatile and widely-used programming language for machine learning, is employed for data preprocessing, feature engineering, and model development.

**📓 Jupyter Notebook:** Jupyter Notebook provides an interactive and collaborative environment to explore and analyze the data, experiment with different algorithms, and fine-tune the model parameters.

**🖥️ Visual Studio Code:** Visual Studio Code, a powerful integrated development environment (IDE), is utilized for writing modular and scalable code. It enables efficient coding practices, debugging, and version control integration with Git, ensuring better collaboration among team members.

**🍃 MongoDB:** MongoDB, a NoSQL document database, is used to store and manage the visa application data. It provides flexibility and scalability for handling large datasets efficiently.

**🐙 GitHub:** GitHub serves as the version control and collaboration platform, allowing team members to work together, track changes, and manage the project's codebase effectively.

**⚡ FLask:** Flask, a modern web framework for building APIs, is used to create a robust and scalable API for serving the machine learning model predictions. It offers high performance and automatic documentation generation.

**☁️ AWS S3:** AWS S3 (Simple Storage Service) is utilized for storing and managing the dataset and other project-related files. It provides secure and scalable cloud storage for easy accessibility and data sharing.

**📦 AWS Elastic Container Registry (ECR):** AWS ECR is a fully managed container registry that makes it easy to store, manage, and deploy Docker container images. By utilizing ECR, you can securely store your machine learning model's containerized image and easily deploy it to AWS services such as AWS Elastic Compute Cloud (EC2).

**⚙️ AWS Elastic Compute Cloud (EC2):** AWS EC2 provides scalable virtual servers in the cloud. You can launch EC2 instances with the desired configuration, including the operating system (e.g., Ubuntu), and deploy your machine learning model on these instances. EC2 offers flexibility and scalability for running the prediction model and handling varying workloads.

**🔒 AWS Identity and Access Management (IAM):** AWS IAM enables you to manage access to AWS services and resources securely. By configuring IAM roles and policies, you can control and grant appropriate permissions to different project team members, ensuring secure access to AWS resources.

**🏃 GitHub Action Runner:** GitHub Actions is a powerful automation and workflow tool that integrates with GitHub repositories. GitHub Action Runner allows you to execute workflows and automate tasks directly on your own infrastructure. By setting up a GitHub Action Runner on an EC2 instance, you can automate tasks like model training, deployment, and testing.

**⚙️Azure Web App:** is a managed PaaS that simplifies building, deploying, and scaling web applications. It supports multiple languages, offers automatic scaling and load balancing, and integrates with CI/CD tools for streamlined deployments.

# AWS-CICD-Deployment-with-Github-Actions
![Logo](https://github.com/Hemanthneu/End-to-End-ML-Project-Student-Metrics/blob/master/US%20VISA%20AWS%20Architechture%20Deployment.jpg)
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

## 4. Create EC2 machine (Ubuntu)

## 5. Open EC2 and Install docker in EC2 Machine:

    #optinal

    sudo apt-get update -y

    sudo apt-get upgrade -y

    #required

    docker --version

    curl -fsSL https://get.docker.com -o get-docker.sh

    sudo sh get-docker.sh

    docker --version

    sudo usermod -aG docker ubuntu

    newgrp docker

# 6. Configure EC2 as self-hosted runner:

    setting>actions>runner>new self hosted runner> choose os> then run command one by one

# 7. Setup github secrets:

- AWS_ACCESS_KEY_ID
- AWS_SECRET_ACCESS_KEY
- AWS_DEFAULT_REGION
- ECR_REPO
