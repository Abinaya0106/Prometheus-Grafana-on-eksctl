# 🚀 EKS Monitoring Setup -- Prometheus & Grafana

## 📖 Project Overview

This project demonstrates setting up a complete Kubernetes monitoring
stack on Amazon EKS using: - EKS (eksctl) - Metrics Server - IRSA (IAM
Roles for Service Accounts) - EBS CSI Driver - Prometheus (Helm) -
Grafana (Helm) - Java Application Monitoring

Includes real-world troubleshooting and production-style setup.

------------------------------------------------------------------------

## 🛠 Tools Used

-   AWS (EKS)
-   Kubernetes
-   eksctl
-   Helm
-   Prometheus
-   Grafana

------------------------------------------------------------------------

## 🔥 Key Learning

-   Debugged Metrics API issues
-   Understood APIService registration
-   Implemented IRSA securely
-   Configured persistent storage with EBS CSI
-   Exposed Grafana via LoadBalancer

------------------------------------------------------------------------

## 🧹 Cleanup

eksctl delete cluster --name eks2 --region us-east-1
