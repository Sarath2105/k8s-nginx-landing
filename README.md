# 🚀 Kubernetes Static Landing Page Deployment

This project demonstrates how to deploy a **dark-themed landing page** using a custom Docker image and Kubernetes (Minikube).

### 🔧 Tech Stack
- Docker (custom NGINX image)
- Kubernetes (Deployment + NodePort Service)
- Docker Hub
- Minikube (local Kubernetes)

---

## 📦 Project Structure

├── Dockerfile
├── landing-deployment.yaml
├── landing-service.yaml
├── static-site/
│ ├── index.html
│ ├── css/
│ ├── js/
│ └── assets/

---

## 🐳 Docker Hub Image

➡️ [`sarath2105/nginx-landing`](https://hub.docker.com/r/sarath2105/nginx-landing)

---

## ⚙️ How to Run

```bash
# Deploy to Kubernetes
kubectl apply -f landing-deployment.yaml
kubectl apply -f landing-service.yaml

# Open the service in browser
minikube service landing-service
