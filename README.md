# Kafka

Deploy the Kafka cluster into the K8s.

## Deploy Kafka Using Helm Chart



```sh
## https://github.com/bitnami/charts/tree/master/bitnami/kafka/
helm repo add bitnami https://charts.bitnami.com/bitnami
helm install kafka-cluster bitnami/kafka \
    -n mizotakhteh --create-namespace \
    --set \
        replicaCount=1
```