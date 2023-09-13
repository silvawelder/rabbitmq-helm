# rabbitmq
📓Documentation: 

## Add the helm chart repo
```bash
helm repo add bitnami https://charts.bitnami.com/bitnami
```
```
helm repo update bitnami
```

## Create a Namespace
```bash 
kubectl create namespace rabbitmq
```
## If necessary check the avaliable versions for this Helm Chart
```bash
helm search repo bitnami/rabbitmq --versions
helm show values bitnami/rabbitmq --version=12.1.4
```

## Install rabbitmq Helm chart

```bash
helm upgrade -i rabbitmq bitnami/rabbitmq \
    --namespace rabbitmq \
    --version v12.1.4 \
    -f rabbitmq-values.yaml
```
