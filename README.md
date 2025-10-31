# 🚀 Spring Boot Java Application

A production-ready **Spring Boot** application containerized with **Docker** and integrated with **Azure Pipelines** for CI/CD.  
This project demonstrates how to build, test, package, and deploy a Java application using modern DevOps practices.

---

## 📦 Features

- ✅ Built with **Spring Boot** (Java 17)
- 🐳 Containerized using **Docker**
- ☁️ Automated CI/CD with **Azure Pipelines**
- 🧪 Maven-based build and dependency management
- 📜 RESTful API-ready architecture
- 🔐 Configurable environment variables for security and flexibility

---

## 🏗️ Project Structure

```bash
springbootjavaapplication/
├── src/                    # Application source code
├── pom.xml                 # Maven build configuration
├── Dockerfile              # Docker image build instructions
├── azurepipeline.yaml      # Azure DevOps pipeline configuration
└── README.md               # Project documentation

⚙️ Requirements

Before you begin, make sure you have the following installed:

Java 17+

Maven 3.8+

Docker

Git

Azure DevOps account (for pipeline builds)

🧰 Setup Instructions
1️⃣ Clone the repository

git clone https://github.com/Brian432-cpu/springbootjavaapplication.git
cd springbootjavaapplication

2️⃣ Build the project with Maven

./mvnw clean package

3️⃣ Run locally

java -jar target/*.jar

Your application will start on http://localhost:8080
.

🐳 Build & Run with Docker
Build the Docker image

docker build -t springbootjavaapp .

Run the container

docker run -p 8080:8080 springbootjavaapp

🧩 Azure Pipeline CI/CD

This project includes an azurepipeline.yaml file that automates:

Code checkout

Maven build and testing

Docker image creation

Push to container registry (e.g., Azure Container Registry or Docker Hub)

You can integrate it with Azure DevOps by connecting your GitHub repo and creating a new pipeline.

🧠 Environment Variables
Variable	Description	Example
SERVER_PORT	Port where the app runs	8080
DB_URL	Database connection URL	jdbc:mysql://localhost:3306/db
DB_USER	Database username	admin
DB_PASS	Database password	password

🧪 Testing

Run unit tests with:

./mvnw test

🚀 Deployment

You can deploy this container image to:

Azure Web App for Containers

Azure Kubernetes Service (AKS)

Docker Hub

Any cloud VM

🧑‍💻 Author

Brian Sumba
📍 Nairobi, Kenya
💼 https://github.com/Brian432-cpu

🧠 Passionate about Cloud Engineering, DevOps, and Cybersecurity

📄 License

This project is licensed under the MIT License
.

🌟 Acknowledgements

Spring Boot Documentation

Azure Pipelines

Docker Docs
