CI/CD Pipeline Project

GitHub + Jenkins + Docker + Kubernetes

📌 Project Overview

This project demonstrates a complete CI/CD (Continuous Integration & Continuous Deployment) pipeline using modern DevOps tools. Whenever code is pushed to GitHub, Jenkins automatically builds a Docker image, pushes it to Docker Hub, and deploys the application to a Kubernetes cluster.

The application used is a simple Python Flask web application, which makes it easy to understand the CI/CD workflow.

🛠️ Technologies Used

GitHub – Source code management

Jenkins – CI/CD automation

Docker – Containerization

Docker Hub – Container image registry
Docker Workflow

Application code is packaged into a Docker image using a Dockerfile

Image is tagged and pushed to Docker Hub

Docker image is later pulled by Jenkins and Kubernetes
📂 Project Structure
ci-cd-pipeline-project/
│
├── app/
│   ├── app.py                 # Flask application source code
│   └── requirements.txt       # Python dependencies
│
├── Dockerfile                 # Docker configuration to build image
├── Jenkinsfile                # Jenkins CI/CD pipeline script
│
├── k8s/
│   ├── deployment.yaml        # Kubernetes Deployment configuration
│   └── service.yaml           # Kubernetes Service configuration
│
└── README.md                  # Project documentation

http://localhost:5000



Kubernetes (Minikube) – Container orchestration

Python Flask – Web application
