
---

## 📝 نمونه فایل `pods.md`
```markdown
# 🐳 Pods Cheatsheet

### لیست پادها
```bash
kubectl get pods
kubectl get pods -o wide
kubectl get pods -n my-namespace

###ساخت پاد از فایل YAML
kubectl apply -f pod.yaml
###حذف پاد
kubectl delete pod mypod
###ورود به داخل پاد
kubectl exec -it mypod -- /bin/bash
###گرفتن لاگ‌ها
kubectl logs mypod
kubectl logs -f mypod
