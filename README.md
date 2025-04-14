# Task 5 - Kubernetes with Minikube

## Objective
Deploy and manage an application on a local Kubernetes cluster using Minikube.

## Tools Used
- Minikube
- kubectl
- Docker

## Steps Performed

1. **Started Minikube cluster**
2. **Deployed Nginx using a Deployment**
3. **Exposed it using a NodePort Service**
4. **Accessed the Nginx app in the browser**
5. **Scaled the deployment to 4 replicas**
6. **Described deployment and fetched pod logs**

## Files
- `deployment.yaml`: Nginx deployment
- `service.yaml`: NodePort service to expose the app

## Screenshots
All screenshots are in the `screenshots/` folder:
- Pods list
- Service output
- Nginx in browser
- Scaled pods
- Describe deployment
- Pod logs

## How to Run
```bash
minikube start
kubectl apply -f deployment.yaml
kubectl apply -f service.yaml
minikube service my-app-service
