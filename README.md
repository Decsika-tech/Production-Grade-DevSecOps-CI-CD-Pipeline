# Production-Grade-DevSecOps-CI-CD-Pipeline
 This project demonstrates an end-to-end DevSecOps pipeline for deploying a secure E-commerce application using CI/CD, containerization, and Kubernetes on AWS.

## Features 
- Automated CI/CD pipeline using Jenkins
- Infrastructure creation using Terraform
- Docker containerization
- Security scanning (Trivy, OWASP)
- Code quality check using SonarQube
- GitOps deployment using ArgoCD
- Kubernetes deployment on AWS EKS
- Fully automated build → scan → deploy flow

## Architecture Diagram
![Production-Grade-DevSecOps-CI-CD-Pipeline](architecture.png)

## Technologies used
- AWS (EKS, EC2, IAM)
- Terraform
- Jenkins
- Docker
- Kubernetes
- ArgoCD
- SonarQube
- Trivy (Image Scan)
- OWASP Dependency Check
- GitHub

## Folder Structure


## How to Run the Project
Follow these steps to run the project.

### Step 1: Clone the Repository

```bash
git clone https://github.com/Decsika-tech/Production-Grade-DevSecOps-CI-CD-Pipeline.git
```
### Step 2: Create an AWS EC2 Instance
- Launch an Ubuntu 24 EC2 instance (t2.large or m7i-flex.large).
- Allocate 50 GB storage.
- Attach an IAM role with Administrator access.
  
### Step 3: Connect to the EC2 Instance

```bash
ssh -i <key.pem> ubuntu@<ec2-public-ip>
sudo -s
hostnamectl set-hostname grocery
sudo -i
```

### Step 4: Install Required Tools
Install the following tools on the EC2 instance:

- Docker
- Jenkins
- Java
- SonarQube 
- AWS CLI
- kubectl
- Terraform

### Step 4: Configure Jenkins Jobs

Create two Jenkins pipeline jobs:

1. **EKS Job** – Creates the Amazon EKS cluster.
2. **Grocery Job** – Builds and deploys the Grocery(E-commerce) application.



## Screenshot


## Contributing
Pull requests are welcome! If you find any issues, feel free to open an issue.

## Contact
For any queries, reach out at helendecsika5@gmail.com.
