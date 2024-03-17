---
tags:
  - CompSci/dev/backend/container/K8s/object
---
# K8s Deployment
### Description:
- [[Deployment]]
- Manages a set of [[K8s pod|pods]] by describing the desired state thru [[K8s ReplicaSet]] by sending configurations to it
	- when update deployment, it mades new replicaset then turn on pods in it and delete in old one
- Represents a group of replicas of the same Pod and keeps your Pods running even when the nodes they run on fail.
- Heterogeneous deployments:
	- typically involve connecting two or more distinct infrastructure environments or regions to address a specific technical or operational need. 
	- called "hybrid", "multi-cloud", or "public-private", depending upon the specifics of the deployment.
- Kubernetes creates a Service with a fixed IP address for your Pods, and a controller says 
	- "I need to attach an external [[Load balancing|Load balancer]] with a public IP address to that Service so others outside the cluster can access it." 
- Master node vs workder note
```yaml
apiVersion: apps/v1
kind: Deployment
metadata:
  name: nginx-deployment
spec:
  selector:
    matchLabels:
      app: nginx
  replicas: 2 # tells deployment to run 2 pods matching the template
  template:
    metadata:
      labels:
        app: nginx # key-value pairs used in kubectl command
    spec:
      containers:
      - name: nginx
        image: nginx:1.14.2
        ports:
        - containerPort: 80
```
### Create deployment
- kubectl create deployment --image nginx nginx-1
	- When a repository isn't specified, the default behavior is to try and find the image either locally or in the Docker public registry. In this case, the image is pulled from the Docker public registry.