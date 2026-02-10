# Kubernetes Basics – Advantages & Architecture

This repository documents my learning notes on **Kubernetes fundamentals**, focusing on its advantages and core architecture components.

---

## 🚀 Advantages of Kubernetes

### 1. Centralized Management
Kubernetes provides centralized management of containers across multiple container hosts.  
It allows:
- Creating containers
- Deleting containers
- Upgrading applications

---

### 2. Container & Node State Management
Kubernetes continuously maintains the desired state of:
- Containers (Pods)
- Nodes

If a container or node fails, Kubernetes automatically works to restore the expected state.

---

### 3. High Availability & Failover
Kubernetes operates in a clustered environment, ensuring:
- High availability
- Automatic failover
- No single point of failure

---

### 4. Resource & Scheduling Management
Efficient scheduling of workloads based on:
- CPU
- Memory
- Node availability

---

### 5. Scalability
Kubernetes supports:
- Manual scaling
- Automatic scaling using Horizontal Pod Autoscaler (HPA)

---

### 6. Application Rollout & Rollback
Supports controlled deployment strategies with:
- Versioned rollouts
- Easy rollback in case of failure

---

### 7. User-Based Access Control
Role-Based Access Control (RBAC) ensures secure and controlled access to cluster resources.

---

## 🏗 Kubernetes Architecture – Key Components

### Master Node (Control Plane)
Responsible for managing the Kubernetes cluster.

#### kube-apiserver
- Entry point to the cluster
- Handles authentication and authorization
- Validates API requests

#### etcd
- Distributed key-value datastore
- Stores cluster state and configuration

#### kube-scheduler
- Selects the best-fit worker node for Pods

#### kube-controller-manager
- Maintains the desired state of the cluster
- Communicates with worker nodes

---

### Worker Nodes
Machines where application workloads run.

#### Container Runtime
Examples:
- Docker
- containerd
- CRI-O

#### kubelet
- Kubernetes agent on each node
- Receives instructions from the master node
- Manages Pods and containers

#### kube-proxy
- Handles networking
- Manages service routing and load balancing

---

## 📌 Author
**Manoj Mishra**  
Network Engineer transitioning into **Cloud, Kubernetes & DevOps**

---
