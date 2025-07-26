# 📦 Kubernetes YAML Manifests Collection

A structured set of Kubernetes YAML examples covering foundational concepts — from namespaces to environment variables and config maps. Ideal for learning, testing, and DevOps portfolio building.

---

## 🗂️ File Structure & Purpose

| 📄 File Name              | 🧠 Purpose                                                              |
|---------------------------|--------------------------------------------------------------------------|
| `01-namespace.yaml`       | 🏷️ Creates a **Namespace** to isolate project resources                  |
| `02-pod.yaml`             | 🧱 Defines a **basic Pod** with a single container                       |
| `03-multi-container.yaml` | 🤝 Deploys a **Pod with multiple containers** (e.g., app + sidecar)      |
| `04-labels.yaml`          | 🔖 Adds **labels** to help identify and group resources                  |
| `05-annotations.yaml`     | 🗒️ Adds **annotations** (non-identifying metadata)                       |
| `06-resources.yaml`       | ⚙️ Sets **CPU & Memory limits/requests** for containers                  |
| `07-env.yaml`             | 🌱 Injects **environment variables** into containers                     |
| `08-config-map.yaml`      | 📑 Creates a **ConfigMap** for external app configurations               |
| `09-pod-config.yaml`      | 🔗 Connects **ConfigMap** to Pod using `envFrom`                         |
| `10-secret.yaml`          | 🔐 Creates a **Secret** for sensitive data like passwords                |
| `11-pod-secret.yaml`      | 🔑 Uses **Secret values** in a Pod as environment variables              |
| `12-service.yaml`         | 🌐 Exposes Pod using **ClusterIP Service** (internal access)             |
| `13-service-np.yaml`      | 🚪 Exposes Pod externally using a **NodePort Service**                   |
| `14-service-LB.yaml`      | 🧲 Provisions a **LoadBalancer Service** (cloud provider required)       |
| `15-replicaset.yaml`      | ♻️ Creates a **ReplicaSet** to maintain a fixed number of Pods           |
| `16-deployment.yaml`      | 🚀 Manages Pods using **Deployment** (supports rollout & rollback)       |

## 🚀 How to Apply

Apply individual manifests:
```bash
kubectl apply -f <file-name>.yaml
