# kubecost-quickstart
Quickly install kube-state-metrics, prometheus, and grafana on your cluster with helm. Requires a helm installation.

> git clone https://github.com/AjayTripathy/kubecost-quickstart.git
> cd kubecost-quickstart

We package a suggestion for roles for your helm service.From the kubecost-quickstart directory, run:

> kubectl apply -f helm.yaml 

After running this, or if you have your own helm service roles already set up, run:

> helm install --debug --dry-run cost-analyzer --name cost-analyzer --namespace monitoring

View the dashboard locally with

> kubectl port-forward --namespace monitoring  deployment/cost-analyzer-grafana 3000

Sample Cluster Dashboard Here:

![Sample Dashboard](https://cdn-images-1.medium.com/max/800/1*rQI3-gKtgKwHSs7JgIdorw.png) 



