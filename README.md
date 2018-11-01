# kubecost-quickstart
Quickly install kube-state-metrics, prometheus, and grafana on your cluster with helm. Requires a helm installation.

> kubectl apply -f helm.yaml 

sets up a suggestion for roles for your helm service

> helm install cost-analyzer --name cost-analyzer --namespace monitoring

View the dashboard locally with

> kubectl port-forward --namespace monitoring  deployment/cost-analyzer-grafana 3000

Sample Cluster Dashboard Here:

![Sample Dashboard](https://cdn-images-1.medium.com/max/800/1*rQI3-gKtgKwHSs7JgIdorw.png) 



