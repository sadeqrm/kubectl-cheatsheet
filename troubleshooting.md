
---

## 📝 `troubleshooting.md`
```markdown
# 🛠️ Troubleshooting

### بررسی وضعیت پاد
```bash
kubectl describe pod mypod
kubectl get pod mypod -o yaml

### CrashLoopBackOff
kubectl logs mypod --previous

### ImagePullError
kubectl describe pod mypod | grep -i image

### بررسی eventها
kubectl get events --sort-by=.metadata.creationTimestamp

### لاگ kube-system
kubectl logs -n kube-system pod/kube-dns
