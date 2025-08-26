
---

## 📝 `services.md`
```markdown
# 🌐 Services

### لیست سرویس‌ها
```bash
kubectl get svc
ساخت سرویس ClusterIP
apiVersion: v1
kind: Service
metadata:
  name: my-service
spec:
  selector:
    app: my-app
  ports:
    - protocol: TCP
      port: 80
      targetPort: 8080
  type: ClusterIP


ساخت سرویس NodePort
spec:
  type: NodePort
  ports:
    - port: 80
      targetPort: 8080
      nodePort: 30007

