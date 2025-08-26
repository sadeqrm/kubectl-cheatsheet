
---

## 📝 `deployments.md`
```markdown
# 📦 Deployments

### لیست Deploymentها
```bash
kubectl get deployments

### ساخت Deployment
kubectl apply -f deployment.yaml

### مقیاس‌دهی (Scaling)
kubectl scale deployment my-deployment --replicas=5

### آپدیت Deployment
kubectl set image deployment/my-deployment nginx=nginx:1.25

### مدیریت Rollout
kubectl rollout status deployment/my-deployment
kubectl rollout history deployment/my-deployment
kubectl rollout undo deployment/my-deployment

