# kubernetes ingress

# what is ingress

## external service vs ingress

# yaml config file 
## example (external service)
```yaml
apiVersion: v1
kind: Service
metadata:
    name: myapp-external-service
spec:
    selector:
        app: myapp
    type: LoadBalancer
    ports:
        - protocol: TCP
          port: 8080
          targetPort: 8080
          nodePort: 35010
```
## example : Ingress
```yaml
apiVersion: v1
kind: Ingress
metadata:
    name: myapp-ingress
spec:
    rules:
    - host 
```
- routing rules forward request to the internal service