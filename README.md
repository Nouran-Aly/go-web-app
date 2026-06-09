# 🚀 Go Web Application - End-to-End DevOps CI/CD Pipeline (EKS + GitOps)

This project demonstrates a complete **production-grade DevOps CI/CD pipeline** for a Go web application deployed on **AWS EKS Kubernetes cluster**, using modern DevOps tools including **Docker, Kubernetes, Helm, GitHub Actions, and Argo CD (GitOps)**.

---

# 🧠 Architecture Overview

The system follows a full GitOps-based CI/CD workflow:
GitHub → GitHub Actions → Docker Build → Container Registry → Argo CD → Kubernetes (EKS) → NGINX Ingress → Application


---

# 🛠️ Tech Stack

- **Backend:** Go (Golang)
- **Containerization:** Docker (Multi-stage build)
- **Orchestration:** Kubernetes (AWS EKS)
- **CI:** GitHub Actions
- **CD:** Argo CD (GitOps)
- **Packaging:** Helm Charts
- **Ingress Controller:** NGINX Ingress Controller
- **Cloud Provider:** AWS (EKS, VPC, Subnets, Security Groups, EC2)

---

# 🚀 Features Implemented

## 🐳 Containerization
- Multi-stage Docker build for optimized production image
- Lightweight and secure container setup

## ☸️ Kubernetes Deployment
- Deployment, Service, and Ingress resources
- Scalable application running on AWS EKS
- External access via Ingress Controller

## 📦 Helm Charts
- Parameterized Kubernetes deployments
- Separate configurations for dev and production environments

## 🔁 CI Pipeline (GitHub Actions)
- Automated linting using golangci-lint
- Build and test Go application
- Docker image build and push to registry

## 🚀 CD Pipeline (Argo CD - GitOps)
- Continuous deployment using GitOps principles
- Automatic sync between Git repository and Kubernetes cluster
- Self-healing and declarative deployments

## 🌐 Networking
- NGINX Ingress Controller for routing traffic
- Host-based routing using custom domain
- AWS VPC networking integration

---


---

# ⚙️ CI/CD Workflow

## 1. Continuous Integration (GitHub Actions)
On every push to main branch:
- Lint Go code (golangci-lint)
- Run tests
- Build Docker image
- Push image to container registry

## 2. Continuous Deployment (Argo CD - GitOps)
- Watches Git repository
- Automatically syncs Kubernetes manifests
- Deploys updates to AWS EKS cluster
- Ensures cluster state matches Git state

---

# ☸️ Kubernetes Architecture

The cluster includes:

- **Deployment:** Runs Go application pods
- **Service:** Internal service communication
- **Ingress:** Exposes application externally via NGINX
- **Helm:** Manages environment-based deployments

---

# 🌐 Application Access

The application is exposed using:

- NGINX Ingress Controller
- AWS EKS worker nodes
- Host-based routing (e.g. `go-web-app.local`)

---

# 📸 Screenshots (Proof of Work)

## 🧠 Architecture Diagram
<img width="2752" height="1536" alt="image" src="https://github.com/user-attachments/assets/4becfac0-773f-485f-8ead-22c1c05acf6e" />

## ⚙️ GitHub Actions CI Pipeline
<img width="1899" height="557" alt="image" src="https://github.com/user-attachments/assets/e69a1c6d-5102-46b5-a5d6-5e06c237ca7b" />

## ☸️ AWS EKS Cluster Resources
<img width="1919" height="945" alt="image" src="https://github.com/user-attachments/assets/bb6edcd2-c0d2-48cf-9c9d-1e616bbf3de7" />

## 🚪 Ingress Working
<img width="1920" height="697" alt="image" src="https://github.com/user-attachments/assets/440f4244-ec95-4890-81d6-fb325f8ad1ff" />

## 🚀 Argo CD Dashboard (GitOps)
<img width="1920" height="961" alt="image" src="https://github.com/user-attachments/assets/8c96078f-943f-4f6e-b607-2b875ab95e6c" />


---

# 📊 What I Learned

- Designing scalable cloud-native architectures
- Kubernetes workload management on AWS EKS
- CI/CD automation using GitHub Actions
- GitOps workflow using Argo CD
- Helm-based configuration management
- Ingress networking and service exposure
- AWS VPC and networking for Kubernetes

---

# 🚀 Future Improvements

- Add HTTPS using AWS ACM
- Replace NGINX Ingress with AWS ALB Ingress Controller
- Add monitoring (Prometheus + Grafana)
- Add centralized logging (EFK stack)
- Add automated rollback strategies in CD pipeline

---

# 👩‍💻 Author
**Nouran Ali**  
