Grafana Loki Configuration
 Source Repo: https://github.com/grafana/loki/blob/main/production/helm/loki/values.yaml

OPENTELEMETRY HELM CHART:
https://github.com/open-telemetry/opentelemetry-helm-charts/blob/main/charts/opentelemetry-collector/values.yaml

 Grafana Helm Charts

 https://github.com/grafana/helm-charts

 Promtail
 https://github.com/grafana/helm-charts/blob/main/charts/promtail/Chart.yaml

 Loki S3 Storage
 https://grafana.com/docs/loki/latest/configure/#s3_storage_config


 Installation using helm

helm dependency update
helm repo update
helm install observability . -f values.yaml



upgrade:
helm upgrade observability . -f values.yaml

ARGOCD
kubectl port-forward service/my-argo-cd-argocd-server -n argocd 8080:443


Grafana
observability-grafana
kubectl port-forward service/observability-grafana 3000:80