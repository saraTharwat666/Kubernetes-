# ☸️ The Kubernetes Mastery Lab
![Kubernetes Banner](https://raw.githubusercontent.com/kubernetes/kubernetes/master/logo/logo.png)

> **"Infrastructure is code, and code is a journey."**  
> This repository is a living documentation of my journey through the Kubernetes ecosystem—from basic pod orchestration to complex cloud-native architectures.

---

## 📽️ Deployment in Action
![K8s Deployment GIF](https://media.giphy.com/media/v1.Y2lkPTc5MGI3NjExNHJueXN4Z3ZqbmZ4Z3ZqbmZ4Z3ZqbmZ4Z3ZqbmZ4Z3ZqJmVwPXYxX2ludGVybmFsX2dpZl9ieV9iZCBmcm9tX2dpcGh5/3o7TKMGpxxy6L_7S0w/giphy.gif)

---

## 🗺️ Roadmap & Progress
I am following a structured path to master K8s. Here is where I stand:

- [x] **Phase 1: Core Concepts** (Pods, ReplicaSets, Deployments)
- [x] **Phase 2: Networking & Services** (ClusterIP, NodePort, LoadBalancer)
- [x] **Phase 3: Storage & Persistence** (PV, PVC, StorageClasses)
- [ ] **Phase 4: Advanced Configuration** (ConfigMaps, Secrets, Ingress)
- [ ] **Phase 5: Package Management** (Helm Charts)
- [ ] **Phase 6: Observability** (Prometheus & Grafana)

---

## 📂 Laboratory Index
Below is a categorized list of all scenarios implemented in this cluster:

### 🏛️ Architecture & Workloads
| Lab Name | Description | Tools Used |
| :--- | :--- | :--- |
| [Guestbook App](./Guestbook-App) | Multi-tier Redis Master-Slave application. | Redis, PHP, NodePort |
| [Nginx Sidecar](./Nginx-Sidecar) | Implementing the Sidecar pattern for PHP-FPM. | Shared Volumes, ConfigMaps |

### 💾 Data & Storage
| Lab Name | Description | Status |
| :--- | :--- | :--- |
| [Drupal-MySQL](./Drupal-MySQL) | Persistent CMS deployment with PV/PVC. | ✅ Completed |
| [Storage Policies](./Storage) | Testing different AccessModes (RWO, RWX). | ⏳ In Progress |

---

## 🛠️ My DevOps Toolbox
- **Orchestration:** Kubernetes (K8s)
- **Scripting:** Bash, YAML
- **Cloud Providers:** Azure, AWS
- **Version Control:** Git & GitHub

---

## 📜 How to Use This Repo
1. **Clone the repository:**
   ```bash
   git clone [https://github.com/YourUsername/k8s-labs.git](https://github.com/YourUsername/k8s-labs.git)
   ```

Navigate to a specific lab:

```Bash
cd MySQL-Drupal
```
Apply the manifests:
```Bash
kubectl apply -f
```
