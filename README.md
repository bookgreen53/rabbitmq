# 🚀 Rabbit Deployment  ( Single  Node ) | 🚀 Rabbit Statefulset ( Cluster Mode )

This repository contains **Kubernetes deployment configurations** for running **Rabbitmq3-Management** in two different modes:

- 🧩 **Single-node mode**   — simple , lightweight , ideal for development.
- ⚙️ **Cluster-style mode**  — provides replication and higher availability.

---

## 📁 Files Overview

| File | Description           |
|------|-----------------------|
| `rabbitmq-one-node.yml`      | Runs Rabbitmq as a single standalone instance. |
| `rabbitmq-cluster-node.yaml` | Deploys Rabbitmq (3replica) nodes for redundancy and basic clustering. |
---

## 🧠 Single Node Deployment (`rabbitmq-one-node.yml`)

### 🧾 Description
This configuration deploys one **Rabbitmq3-management** instance in Kubernetes.
It’s designed for:
- local testing
- development environments
- lightweight caching

### 🧩 Apply the configuration
```bash
kubectl apply -f rabbitmq-one-node.yml
```
### 🧩
```bash
kubectl get pods -l app=rabbitmq
kubectl get svc rabbitmq-svc
```
---
## 🧠 Cluster Mode Deployment (`rabbitmq-cluster-node.yaml`)

### 🧾 Description
This configuration deploys one **Rabbitmq3-management** instance in Kubernetes.
It’s designed for:
- local testing
- development environments
- lightweight caching

### 🧩 Apply the configuration
```bash
kubectl apply -f rabbitmq-cluster-node.yaml
```
### 🧩
```bash
kubectl get pods -l app=rabbitmq
kubectl get svc rabbitmq-svc
```
*** Point :  these are For Default Namespace in k8s.
