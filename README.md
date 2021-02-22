# Prometheus and Grafana monitoring @fint

## Install
```shell
kubectl apply -f namespace.yaml
helm install -f prometheus-values.yaml prometheus prometheus-community/prometheus --namespace monitoring
helm install -f grafana-values.yaml grafana grafana/grafana --namespace monitoring
```

## Upgrade
```shell
helm upgrade -f prometheus-values.yaml prometheus prometheus-community/prometheus --namespace monitoring
helm upgrade -f grafana-values.yaml grafana grafana/grafana --namespace monitoring
```



## Links

- https://grafana.com/docs/grafana/latest/auth/azuread/
