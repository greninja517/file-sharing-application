# 📁 File Sharing App (Deployed with Kubernetes & Helm)

A simple, secure web application for sharing files using unique PINs. This project demonstrates the deployment of a pre-existing three-tier application (JavaScript frontend, Spring Boot backend, MySQL database) onto a Kubernetes cluster (Amazon EKS and Minikube) using Docker, Helm, and a Jenkins CI/CD pipeline.

---

## 🌟 Application Features

*   ⬆️ **File Upload**: Easily upload a single file.
*   🔑 **PIN Generation**: Automatically generates a unique, secure PIN for every upload.
*   🔒 **Secure Download**: Files are only accessible with the correct PIN.
*   👤 **No Signup Required**: Quick and anonymous file sharing.

---

## 🛠️ Technologies Used

*   **Application Stack**:
    *   Frontend: HTML, JavaScript, Tailwind CSS
    *   Backend: Spring Boot (Java 17)
    *   Database: MySQL
*   **Containerization & Orchestration**:
    *   Docker
    *   Kubernetes
    *   Helm
*   **CI/CD**:
    *   Jenkins
*   **Cloud Platform & Services**:
    *   AWS EKS (Elastic Kubernetes Service)
    *   AWS ECR (Elastic Container Registry)
*   **Local Development Environment**:
    *   Minikube

---

## 🚀 Deployment

You can deploy this application to your Kubernetes cluster (Minikube recommended for local testing) using the published Helm chart.
**HELM Chart source code here**: https://github.com/greninja517/file-sharer.git

### Prerequisites

*   A running Kubernetes cluster (e.g., Minikube, kind).
*   `kubectl` command-line tool installed and configured.
*   `helm` command-line tool (v3+) installed.

### Step 1: Add the Helm Repository

Add the Helm repository where the File Sharing App chart is hosted:
```bash
helm repo add file-sharer https://greninja517.github.io/file-sharer/
helm repo update
```

### Step 2. Install the Helm Chart

Install the file-sharing-app chart into your Kubernetes cluster:
```bash
helm install file-sharing-app file-sharer/file-sharer --namespace file-sharing --create-namespace
```

### 3. Accessing the Application
Now, you can access the application at http://file.cloud-ninja.xyz:80/ ( If you haven't changed the `ingress.domain_name` variable using the --set option while installing the helm chart.)

---

## 🔗 Helm Chart Repository
This repository contains the Helm chart source files and is published via GitHub Pages at:
➡️ **https://greninja517.github.io/file-sharer/**

---