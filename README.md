# 🚀 CI/CD Pipeline for Node.js App using Jenkins, Docker, SonarQube & Trivy

## 📌 Project Overview
This project demonstrates an automated **CI/CD pipeline** to deploy a Node.js application using:
- Jenkins
- Docker
- SonarQube
- Trivy
- AWS EC2
- GitHub

---

## ⚙️ Steps

### 1. Setup Infrastructure
- Launched **AWS EC2 instance**
- Installed **Docker & Git**

### 2. Setup SonarQube
- Ran SonarQube container
- Configured SonarQube project
- Integrated Jenkins with SonarQube

### 3. Setup Jenkins
- Installed Jenkins on EC2
- Installed required plugins:
  - SonarQube Scanner
  - Pipeline
  - Docker
- Configured credentials for:
  - DockerHub
  - SonarQube

### 4. Pipeline Flow
1. Clean workspace  
2. Checkout code from GitHub  
3. Run SonarQube analysis  
4. Wait for Quality Gate result  
5. Build Docker image  
6. Run Trivy scan  
7. Push Docker image to DockerHub  
8. Deploy application  

### 5. Deployment
- Application deployed inside Docker container  
- Running on **port 3000**  

---

## 📂 Repo Structure



