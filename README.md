# 🚀 Kubernetes App Deployment using Minikube

## 📌 Project Overview

This project demonstrates how to deploy a containerized application on a local Kubernetes cluster using Minikube.

## 🧰 Tech Stack

* Docker
* Kubernetes
* Minikube
* kubectl

## 🏗️ Architecture

Browser → Service (NodePort) → Deployment → Pods → Container

## ⚙️ Setup Instructions

### 1. Start Minikube

```bash
minikube start --driver=docker
```

### 2. Use Minikube Docker

```bash
eval $(minikube docker-env)
```

### 3. Build Docker Image

```bash
docker build -t myapp:v1 ./app
```

### 4. Deploy to Kubernetes

```bash
kubectl apply -f k8s/deployment.yaml
kubectl apply -f k8s/service.yaml
```

### 5. Access Application

```bash
minikube service myapp-service
```

## 📊 Outputs

* Running Pods
* Exposed Service
* Browser Output

## 🚀 Features

* Containerized app using Docker
* Kubernetes Deployment & Service
* Scalable architecture
* Local cluster using Minikube


## 🎯 Learning Outcome

* Kubernetes fundamentals
* Deployment & Service concepts
* Docker + Kubernetes integration
* Real DevOps workflow

---

⭐ This project is part of my DevOps learning journey.
