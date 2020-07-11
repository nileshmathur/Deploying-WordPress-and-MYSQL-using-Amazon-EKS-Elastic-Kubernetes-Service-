######################################################################### 
Deploying-WordPress-and-MYSQL-using-Amazon-EKS-Elastic-Kubernetes-Service-
This is a project created in which WordPress and MYSQL is deployed using Amazon EKS 
EFS Provisioner is created and PVC is attached to it
WordPress is deployed using Service Type "Load Balancer" on port 80 which allows outside connectivity using Apache httpd server
WordPress image "wordpress:4.8-apache" is used for launching containers and its environment variables are declared in a secret file which is not shared for security purposes
MYSQL is deployed using Service Type "ClusterIP" on port 3306 which does not allow outside connectivity because MYSQL Container contains sensitive data
WordPress image "mysql:5.6" is used for launching containers and its environment variables are declared in a secret file which is not shared for security purposes
