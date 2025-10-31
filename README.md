# 🚀 Spring Boot Docker Application with Azure DevOps

This is a simple **Spring Boot** application containerized with **Docker** and deployed using **Azure DevOps Pipelines**.

---

## 🧱 Project Overview

This project demonstrates how to:
- Build a Spring Boot application with Maven
- Containerize the app using Docker
- Push the Docker image to a container registry (DockerHub or ACR)
- Automate the build and push process using Azure DevOps CI/CD pipeline

---

## 📂 Folder Structure

spring-boot-docker/
├── src/ # Java source code
├── pom.xml # Maven build file
├── Dockerfile # Docker configuration
├── azurepipeline.yaml # Azure DevOps pipeline definition
└── README.md # Project documentation


---

## ⚙️ Run Locally

1. Clone this repository:
   ```bash
   git clone https://github.com/Brian432-cpu/springbootjavaapplication.git
   cd springbootjavaapplication


Build the project:

 :mvn clean package

Run the Spring Boot app:

:java -jar target/*.jar
:Access it at http://localhost:8080


🐳 Docker Usage

:docker build -t springbootapp:latest .

Run Container:

docker run -d -p 8080:8080 springbootapp:latest

🔧 Azure DevOps Pipeline

The pipeline (azurepipeline.yaml) has two stages:

Build – Builds the app and Docker image

Push – Pushes the image to a container registry


☸️ Kubernetes (Optional)

If you want to deploy this app on Kubernetes later, create manifest files:

deployment.yaml

service.yaml

Then deploy using:

:kubectl apply -f k8s/

👨‍💻 Author

Brian Sumba

💻 https://github.com/Brian432-cpu

☁️ Azure DevOps: kissingersumba1

✉️ Passionate about Cloud, DevOps, and Cybersecurity

“Automate, containerize, and deploy with confidence.” 🚢

