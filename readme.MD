# 📦 Kubernetes YAML Manifests Collection

A structured set of Kubernetes YAML examples covering foundational concepts — from namespaces to environment variables and config maps. Ideal for learning, testing, and DevOps portfolio building.

---

## 🗂️ File Structure & Descriptions

# 🗂️ File Structure & Descriptions

| 📄 File Name              | 🔍 Description                                                                 |
|---------------------------|--------------------------------------------------------------------------------|
| `01-namespace.yaml`       | 🏷️ Creates a custom **Namespace** to isolate resources logically.               |
| `02-pod.yaml`             | 🧱 Defines a **basic Pod** with a single container.                             |
| `03-multi-container.yaml` | 🧊 Demonstrates a **Pod with multiple containers** sharing resources.           |
| `04-labels.yaml`          | 🏷️ Adds **Labels** for identification and grouping.                            |
| `05-annotations.yaml`     | 📝 Adds **Annotations** for non-identifying metadata.                          |
| `06-resources.yaml`       | ⚖️ Sets **resource requests and limits** (CPU/memory) for containers.          |
| `07-env.yaml`             | 🌱 Injects **environment variables** into containers.                          |
| `08-config-map.yaml`      | 📘 Creates a **ConfigMap** to externalize configuration.                       |
| `09-pod-config.yaml`      | 🔗 Connects a **Pod to ConfigMap** using environment variables.                 |
| `10-secret.yaml`          | 🔐 Creates a **Secret** to store sensitive information like passwords, tokens. |
| `11-pod-secret.yaml`      | 🧬 Injects a **Secret into a Pod** via environment variables or mounted files.  |
              |

---

## 🚀 How to Apply

Apply individual manifests:
```bash
kubectl apply -f <file-name>.yaml
