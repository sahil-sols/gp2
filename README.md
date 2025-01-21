# ArgoCD AKS Demo

This repository demonstrates an **ArgoCD-based GitOps deployment** for an example application on **Azure Kubernetes Service (AKS)**. It includes **CI/CD pipelines with GitHub Actions**, **network security configurations**, and **scalability features like HPA (Horizontal Pod Autoscaler)**.

---

## 🚀 **Features**
- **ArgoCD for GitOps-based Deployment**
- **GitHub Actions CI/CD**
- **Ingress Controller for External Access**
- **Network Policies for Security**
- **HPA for Auto-scaling**
- **App of Apps pattern for multi-environment deployment**


---

## 🎯 **Pre-requisites**
Before you begin, ensure you have the following:
- **Azure Kubernetes Service (AKS) cluster**
- **Azure Container Registry (ACR)**
- **ArgoCD installed on AKS**
- **kubectl & Helm installed**
- **GitHub repository with Actions enabled**
- **Domain & DNS configured for Ingress**

---

## 🏗 **Setup Instructions**

### **Step 1: Install ArgoCD on AKS**
```sh
kubectl create namespace argocd
kubectl apply -n argocd -f https://raw.githubusercontent.com/argoproj/argo-cd/stable/manifests/install.yaml
