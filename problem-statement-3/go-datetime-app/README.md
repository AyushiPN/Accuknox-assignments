# DateTime App - Kubernetes Deployment

### 📝 Description  
A simple Go application that returns the current date and time, deployed using Kubernetes with **2 replicas** and exposed via a **LoadBalancer** service.  

## 📜 Kubernetes Resources
- **Pods**: 2 replicas running  
- **Service Type**: LoadBalancer  
- **Deployment YAML**: [deployment.yaml](deployment.yaml)  
- **Service YAML**: [service.yaml](service.yaml)  

## 📸 Proof of Running Setup
![image](https://github.com/user-attachments/assets/e3c92af6-06e9-434d-9e4e-a7c1c60c92da)
![image](https://github.com/user-attachments/assets/97cff883-bbdb-434d-beb6-fc7e066bca23)
<img width="931" alt="image" src="https://github.com/user-attachments/assets/e80f89e6-ecdf-4b0d-8daa-e66821904786" />

<img width="843" alt="image" src="https://github.com/user-attachments/assets/a519acaf-56cc-4af0-a1a5-f6da3fbfabbf" />


### Click to view the Docker image -> https://hub.docker.com/repository/docker/ayushi0903/datetime-app/general
### ✅ Running Pods -> pods.txt
### ✅ Running Service -> service.txt

### 🌍 Accessing the Application
The application is exposed via a **LoadBalancer** service.  
To get the current external IP, run:
```sh
kubectl get services datetime-app