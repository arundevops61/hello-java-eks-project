Hello Java EKS Project

This is a small DevOps demo project where I built and deployed a simple Java Hello World application into Kubernetes running on AWS EKS. The goal of this project is to practice and demonstrate real DevOps workflow including build, containerization, CI/CD, and Kubernetes deployment.

About This Project

In this project, I created a basic Java application and deployed it into Kubernetes using Docker and Jenkins pipeline. This project helps in understanding how application code moves from development to production using automation.

Tools & Technologies Used

Java

Maven

Docker

Kubernetes

AWS EKS

Jenkins

Git

Project Folder Structure
hello-java-eks-project
│
├── app → Java source code and pom file
├── Docker → Dockerfile to build container image
├── k8s → Kubernetes deployment and service files
├── jenkins → Jenkins pipeline script
└── README.md

How To Run This Project
Clone Repository
git clone https://github.com/arundevops61/hello-java-eks-project.git
cd hello-java-eks-project

Build Java Application
cd app
mvn clean package

Build Docker Image
docker build -t hello-java-app .

Run Container Locally (Optional)
docker run -p 8080:8080 hello-java-app

Deploy Into Kubernetes
Deploy Application
kubectl apply -f k8s/deployment.yaml

Deploy Service
kubectl apply -f k8s/service.yaml

Verify Deployment
kubectl get pods
kubectl get svc

CI/CD Flow

The Jenkins pipeline performs below steps:

Pull source code

Build Java application

Build Docker image

Push Docker image

Deploy application into Kubernetes

What I Learned From This Project

How to containerize Java application

How Kubernetes deployment works

How CI/CD pipeline automates build and deployment

Understanding end-to-end DevOps workflow

Future Improvements

Add Helm deployment

Add monitoring setup

Add auto scaling

Improve pipeline automation

Author

Arun
DevOps Engineer
