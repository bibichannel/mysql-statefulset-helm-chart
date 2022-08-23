# Use helm deploy release into kubernetes: mysql-statefulset-helm-chart

## Getting Started
- Install **helm** version latest.
- File **config** of kubernetest in **~/.kube** folder.

## Deploy release to k8s
```
helm upgrade --install --config --debug --kubeconfig ~/.kube/config --create-namespace --namespace mysql mysql-statefulset ./
```

## Check release
```
helm list -n mysql
```

## Uninstall release
```
helm uninstall mysql-statefulset -n mysql
```
