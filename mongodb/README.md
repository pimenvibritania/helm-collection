helm repo add bitnami https://charts.bitnami.com/bitnami
helm repo update
helm upgrade --install mongo-rb bitnami/mongodb --namespace rollback --create-namespace -f values.yaml