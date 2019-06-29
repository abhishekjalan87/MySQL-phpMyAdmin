# MySQL-phpMyAdmin
# MySQL Server with PHPMyAdmin

##If someone dont want to use Persistent Volume & Claim, please use only mysqldb-deployment.yaml & mysqldb-svc.yaml

##Command to deploy MySQLDB Server
kubectl create -f mysqldb-pv.yaml

##Command to deploy Persistent Volume Claim for MYSQL
kubectl create -f mysqldb-pvc.yaml

##Command to deploy MySQLDB Server
kubectl create -f mysqldb-deployment.yaml

##Command to deploy MySQLDB Service
kubectl create -f mysqldb-svc.yaml


## Also, you can avoid all above commands and can run single command which will deploy mysqldb-pv, mysqldb-pvc, mysqldb-svc & mysqldb-deployment

##Command to deploy all in one
kubectl create -f mysqldb-single.yaml


# IMP ## Before you deploy PhpMyAdmin please make sure MYSQL Server is already up and running.
##Deploy PhpMyAdmin and connect with your existing MYSQL Server which is running on your K8S env. 
##Make sure you change the root password/HOST/PORT wherever its required.

##Command to deploy PHPMyAdmin:
kubectl create -f PhpMyAdmin.yaml






Later, we will update README file more in details.



