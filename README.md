# 🚀 KubeHealth – Kubernetes-Based Application Health Monitoring & Auto-Scaling System

## 📌 Overview

KubeHealth is a cloud-native project that demonstrates application deployment, monitoring, and auto-scaling using Kubernetes. The system showcases how modern DevOps tools can be used to build scalable, reliable, and efficient application infrastructure.

This project focuses on:

* Containerized application deployment
* Kubernetes orchestration
* Dynamic auto-scaling using HPA
* Monitoring using Prometheus
* Self-healing mechanisms

---

## 🛠️ Technologies Used

* **Docker** – Containerization
* **Kubernetes** – Orchestration platform
* **Prometheus** – Monitoring tool
* **Helm** – Package management
* **Minikube** – Local Kubernetes cluster
* **YAML** – Configuration files

---

## ⚙️ Project Architecture

The system is built using Kubernetes components:

* **Deployment** → Manages application pods
* **ReplicaSet** → Maintains desired number of pods
* **Service** → Exposes application to users
* **HPA (Horizontal Pod Autoscaler)** → Scales pods based on CPU usage
* **Prometheus** → Collects system metrics

---

## 📂 Project Structure

```
KubeHealth-Monitoring-System/
│── README.md
│── deployment.yaml
│── service.yaml
│── hpa.yaml
│── prometheus.yaml
│── screenshots/
```

---

## 🚀 How to Run the Project

1. Start Minikube:

```
minikube start
```

2. Apply Kubernetes configurations:

```
kubectl apply -f deployment.yaml
kubectl apply -f service.yaml
kubectl apply -f hpa.yaml
```

3. Access the application:

```
minikube service kubehealth-service
```

---

## 📊 Monitoring and Visualization

Prometheus is used for monitoring system performance by collecting metrics such as CPU usage, memory consumption, and pod status.

Prometheus scrapes metrics from the Kubernetes cluster and stores them as time-series data.

Visualization can be done using Grafana dashboards (optional), which provide real-time insights into system behavior.

---

## 🔄 Auto-Scaling (HPA)

The Horizontal Pod Autoscaler (HPA) automatically scales the number of pods based on CPU utilization.

* High CPU usage → Increase pods
* Low CPU usage → Decrease pods

This ensures efficient resource utilization and improved application performance.

---

## ♻️ Self-Healing Mechanism

Kubernetes automatically monitors the health of pods.

* If a pod fails → It is terminated
* A new pod is created automatically

This ensures high availability and minimal downtime.

---

## 📸 Screenshots

(Add your screenshots in the `/screenshots` folder)

Example:

* Pods running
* HPA output
* Prometheus dashboard
* Application in browser

---

## 🎯 Features

* Automated deployment using Kubernetes
* Dynamic auto-scaling using HPA
* Real-time monitoring using Prometheus
* Self-healing capability
* High availability system

---

## 🔮 Future Scope

* Integration with Grafana dashboards
* CI/CD pipeline implementation
* Deployment on AWS EKS
* Security using RBAC

---

## 📚 Conclusion

This project demonstrates how Kubernetes and monitoring tools can be used to build scalable and reliable cloud-native systems. It provides practical knowledge of DevOps concepts such as containerization, orchestration, monitoring, and automation.

---

## 👨‍💻 Author

* Neha Jaiswal 
* Lovey Professional University 
* Btech CSE 

---

## 🔗 GitHub Repository

https://github.com/jaiswal-lpu/KubeHealth-Monitoring-System
