# Prometheus Installation

helm repo add prometheus-community
https://prometheus-community.github.io/helm-charts helm repo update

helm install prometheus prometheus-community/prometheus --namespace
prometheus --set alertmanager.persistentVolume.storageClass="gp2" --set
server.persistentVolume.storageClass="gp2"

Access using: kubectl port-forward deployment/prometheus-server
9090:9090 -n prometheus
