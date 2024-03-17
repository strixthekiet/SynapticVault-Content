---
tags:
  - CompSci/dev/backend/container/K8s
---
# Kubernetes Namespaces
### Description:
- A mechanism for isolating groups of resources within a single [[K8s Cluster|cluster]].
- A **multi-tenancy cluster** allows for multiple users or teams to share one cluster for their workloads while maintaining isolation and fair resource sharing. 
- This is achieved by creating **namespaces**. Namespaces allow multiple virtual clusters to exist on the same physical cluster.
- `kubectl get services --namespace=kube-system`
- [Managing a GKE Multi-tenant Cluster with Namespaces | Google Cloud Skills Boost](https://www.cloudskillsboost.google/course_sessions/7226348/labs/451696)
### Initial namespaces:
- `default`
	- Kubernetes includes this namespace so that you can start using your new cluster without first creating a namespace.
- `kube-node-lease`
	- This namespace holds [Lease](https://kubernetes.io/docs/concepts/architecture/leases/) objects associated with each node. Node leases allow the kubelet to send [heartbeats](https://kubernetes.io/docs/concepts/architecture/nodes/#heartbeats) so that the control plane can detect node failure.
- `kube-public`
	- This namespace is readable by _all_ clients (including those not authenticated). This namespace is mostly reserved for cluster usage, in case that some resources should be visible and readable publicly throughout the whole cluster. The public aspect of this namespace is only a convention, not a requirement.
- `kube-system`
	- The namespace for objects created by the Kubernetes system.