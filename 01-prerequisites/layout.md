                👩‍💻 DevOps Engineer
                        |
                        |
                   EC2 Instance
        (AWS CLI, kubectl, eksctl, Helm)
                        |
                        |
                Amazon EKS Cluster
               (2 Worker Nodes)
        ---------------------------------
        |                               |
   Java Application                Metrics Server
        |                               |
        ----------- Metrics -------------
                        |
                   Prometheus
        (Scrapes K8s + App Metrics)
                        |
                        |
                    Grafana
              (LoadBalancer Service)
                        |
                        |
                    Browser