# Super Mario Pod with Log Monitoring

This repository contains the configuration to deploy a Kubernetes Pod running a Super Mario container with a BusyBox sidecar for monitoring Tomcat logs.

## Deployment Instructions

1. **Clone the Repository**

   ```sh
   git clone https://github.com/yourusername/supermario-pod.git
   cd supermario-pod
   ```
   
2. Apply the sidecar manifest
```sh
kubectl apply -f supermario-pod.yaml
```

3. Verify your deployment
```sh
kubectl get pods
```

4. Check busy box logs
```sh
kubectl logs supermario-pod -c busybox-logger
```
