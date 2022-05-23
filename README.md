# nextcloud-kubernetes

Es necesario crear los secrets de la base de datos para que funcione, para ello modificar y ejecutar el siguiente comando.

```
kubectl create secret generic nextcloud-db-secret \
    --from-literal=MYSQL_ROOT_PASSWORD=rootPassw0rd1 \
    --from-literal=MYSQL_USER=nextcloud \
    --from-literal=MYSQL_PASSWORD=passw0rd1
```
    
Fuente: [Blog True Kubernetes](https://blog.true-kubernetes.com/self-host-nextcloud-using-kubernetes/)
