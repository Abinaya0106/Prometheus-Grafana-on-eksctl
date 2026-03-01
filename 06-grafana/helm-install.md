# Grafana Installation

helm repo add grafana https://grafana.github.io/helm-charts helm repo
update

kubectl create namespace grafana

helm install grafana grafana/grafana --namespace grafana --set
persistence.enabled=true --set persistence.storageClassName="gp2" --set
service.type=LoadBalancer

Default Login: Username: admin Password: EKS!sAWSome

Import Dashboard ID: 6417
