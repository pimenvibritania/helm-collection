helm repo add choerodon https://openchart.choerodon.com.cn/choerodon/c7n
helm repo update
helm upgrade --install mysql-rollback choerodon/mysql --version 5.7.0 --namespace rollback --create-namespace -f values.yml