# ☸️ kubectl Cheatsheet

مجموعه‌ای از پرکاربردترین دستورات `kubectl` برای کار با Kubernetes.  
این ریپو برای کسانی که تازه با K8s کار می‌کنن یا دنبال یک راهنمای سریع هستن ساخته شده.  

---

## 📖 محتوا
- [Basics](./basics.md)
- [Pods](./pods.md)
- [Deployments](./deployments.md)
- [Services](./services.md)
- [Troubleshooting](./troubleshooting.md)

---

## ⚡ Quick Reference

```bash
# نمایش همه namespaceها
```
kubectl get ns
```
# لیست همه پادها در یک namespace
kubectl get pods -n my-namespace

# توضیحات یک پاد
kubectl describe pod mypod -n my-namespace

# اجرای دستور داخل پاد
kubectl exec -it mypod -- bash

# گرفتن لاگ‌ها
kubectl logs -f mypod
