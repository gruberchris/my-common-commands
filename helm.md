# Helm Commands

| Command | Description |
| --- | --- |
| helm dependency build | Get Helm dependency charts from registry |
| helm install <chart name> <path to chart> | Install helm chart in Kubernetes |
| helm uninstall <chart name> | Removes helm chart from Kubernetes |
| helm install --dry-run --debug <chart name> <path to chart> | troubleshoot a Helm chart installation |
| helm search <chart name> | find a chart in the Helm registry |
| helm install --values=my-values.yaml <chart name> | install helm chart using values from a specified values.yaml file |
| helm install --set version=2.0.0 | install helm chart as the specified version |
| helm upgrade <chart name> | upgrade specified helm chart |
| helm rollback <chart name> | rollback the specified helm chart |