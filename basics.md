
---

## 📝 `basics.md`
```markdown
# 📘 Basics

### نمایش اطلاعات کلاستر
```bash
kubectl cluster-info
kubectl get nodes

کار با contextها
kubectl config get-contexts
kubectl config use-context my-cluster

کار با namespaceها
kubectl get ns
kubectl create ns my-namespace
kubectl config set-context --current --namespace=my-namespace

