# ☸️ Kubernetes (K8s) Ultimate Cheat Sheet & Labs
![Kubernetes Architecture](https://sookocheff.com/post/kubernetes/understanding-kubernetes-networking-model/internet-to-service.gif)

> **"Mastering the art of container orchestration, one command at a time."**  
> This repository serves as a comprehensive guide to Kubernetes essential commands, architecture, and hands-on laboratory exercises.

---

---

## 🛠️ Essential Kubectl Commands (The Core)

### 🔍 1. Exploration & Troubleshooting
| Command | Description |
| :--- | :--- |
| `kubectl get all` | Show all resources in the current namespace. |
| `kubectl describe pod <pod-name>` | Show detailed information about a specific pod (Events/Logs). |
| `kubectl logs <pod-name>` | Display logs from a container in a pod. |
| `kubectl exec -it <pod-name> -- bin/bash` | Open an interactive terminal inside a pod. |

### 🚀 2. Resource Management
| Command | Description |
| :--- | :--- |
| `kubectl apply -f <file.yaml>` | Create or update resources defined in a YAML file. |
| `kubectl run <name> --image=<image>` | Create a temporary pod for testing. |
| `kubectl scale deployment <name> --replicas=5` | Scale a deployment to a specific number of pods. |
| `kubectl delete -f <file.yaml>` | Remove all resources defined in the YAML file. |

### 🌐 3. Networking & Services
| Command | Description |
| :--- | :--- |
| `kubectl get svc` | List all services and their external/internal IPs. |
| `kubectl expose deployment <name> --port=80 --type=NodePort` | Expose a deployment to external traffic. |
| `kubectl port-forward <pod-name> 8080:80` | Forward a local port to a port on the pod. |

---

## 📁 Repository Roadmap
- [x] **Basics:** Pods, Deployments, and Services.
- [x] **Storage:** Persistent Volumes (PV) and Claims (PVC).
- [ ] **Config:** Secrets, ConfigMaps, and Resource Quotas.
- [ ] **Advanced:** Helm Charts, Ingress Controllers, and Monitoring.

---

## ⚡ Quick DevOps Alias
To speed up your workflow, add this to your `.bashrc` or run it in your terminal:
```bash
alias k='kubectl'
complete -F __start_kubectl k
