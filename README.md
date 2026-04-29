
# Tetris DevSecOps Project

## 📌 Project Overview

This project demonstrates a complete **DevOps CI/CD pipeline** by deploying a containerized Tetris web application using modern DevOps tools and cloud infrastructure.

The goal is to simulate a real-world workflow where code changes automatically trigger build, packaging, and deployment processes.

---

## 🧱 Architecture

GitHub → GitHub Actions → Docker Build → Docker Hub → AWS EC2 Deployment

---

## 🛠️ Tools & Technologies Used

* Git & GitHub (Version Control)
* GitHub Actions (CI/CD Pipeline)
* Docker (Containerization)
* Docker Hub (Image Registry)
* AWS EC2 (Cloud Hosting)
* Linux (Ubuntu Server)

---

## ⚙️ CI/CD Pipeline Workflow

1. Code is pushed to GitHub repository
2. GitHub Actions pipeline is triggered
3. Docker image is built automatically
4. Image is pushed to Docker Hub
5. Application can be deployed on EC2 using the latest image

---

## 🐳 Docker Setup

### Build Image

```bash
docker build -t tetris-app .
```

### Run Container

```bash
docker run -d -p 8080:80 tetris-app
```

---

## ☁️ AWS Deployment

* Created EC2 instance (Ubuntu)
* Installed Docker on EC2
* Pulled Docker image from Docker Hub
* Ran container and exposed application

---

## 🔐 Security

* Docker Hub credentials stored securely using GitHub Secrets
* No hardcoded credentials in code

---

## 📊 Future Enhancements

* Kubernetes deployment (k3s / EKS)
* Monitoring using Prometheus & Grafana
* Security scanning using Trivy
* Infrastructure as Code using Terraform

---

## 🎯 Key Learnings

* CI/CD pipeline automation using GitHub Actions
* Docker image creation and registry management
* Cloud deployment using AWS EC2
* Debugging real-world DevOps issues

---

## 👩‍💻 Author

**Shabin Shareefa**

---

## ⭐ Conclusion

This project showcases a beginner-to-intermediate level DevOps workflow and demonstrates practical knowledge of automation, containerization, and cloud deployment.

---
