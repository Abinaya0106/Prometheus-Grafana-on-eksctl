
## Installing KubeServer Setup:


> --kubectl apply -f https://github.com/kubernetes-sigs/metrics-server/releases/latest/download/components.yaml ~

> --kubectl apply -f components.yaml
 
## Verify that the metrics-server deployment is running the desired number of pods with the following command

> --kubectl get deployment metrics-server -n kube-system

**Errors Occured :**

Error zone : What I broke (Learning)
$ kubectl apply -f https://github.com/kubernetes-sigs/metrics-server/releases/latest/download/components.yaml
Warning: resource serviceaccounts/metrics-server is missing the kubectl.kubernetes.io/last-applied-configuration annotation which is required by kubectl apply. kubectl apply should only be used on resources created declaratively by either kubectl create --save-config or kubectl apply. The missing annotation will be patched automatically.
serviceaccount/metrics-server configured
clusterrole.rbac.authorization.k8s.io/system:aggregated-metrics-reader created
Warning: resource clusterroles/system:metrics-server is missing the kubectl.kubernetes.io/last-applied-configuration annotation which is required by kubectl apply. kubectl apply should only be used on resources created declaratively by either kubectl create --save-config or kubectl apply. The missing annotation will be patched automatically.
clusterrole.rbac.authorization.k8s.io/system:metrics-server configured
Warning: resource rolebindings/metrics-server-auth-reader is missing the kubectl.kubernetes.io/last-applied-configuration annotation which is required by kubectl apply. kubectl apply should only be used on resources created declaratively by either kubectl create --save-config or kubectl apply. The missing annotation will be patched automatically.
rolebinding.rbac.authorization.k8s.io/metrics-server-auth-reader configured
Warning: resource clusterrolebindings/metrics-server:system:auth-delegator is missing the kubectl.kubernetes.io/last-applied-configuration annotation which is required by kubectl apply. kubectl apply should only be used on resources created declaratively by either kubectl create --save-config or kubectl apply. The missing annotation will be patched automatically.
clusterrolebinding.rbac.authorization.k8s.io/metrics-server:system:auth-delegator configured


Why we need metrics server here

Metrics Server collects CPU and memory usage from Kubernetes nodes and pods and exposes it to the Kubernetes Metrics API, enabling commands like kubectl top and autoscaling (HPA).