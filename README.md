# kubecost-quickstart
Quickly install kube-state-metrics, prometheus, and grafana on your cluster with helm. Requires a helm installation.

> kubectl apply -f helm.yaml 

sets up a suggestion for roles for your helm service

> helm install cost-analyzer --name cost-analyzer --namespace monitoring

View the dashboard locally with

> kubectl port-forward --namespace monitoring  deployment/cost-analyzer-grafana 3000



