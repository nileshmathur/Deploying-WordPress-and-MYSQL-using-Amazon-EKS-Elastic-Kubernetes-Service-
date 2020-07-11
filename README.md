(1)Deploying-WordPress-and-MYSQL-using-Amazon-EKS-Elastic-Kubernetes-Service
(2)This is a project created in which WordPress and MYSQL is deployed using Amazon EKS 
(3)EFS Provisioner is created and PVC is attached to it
(4)WordPress is deployed using Service Type "Load Balancer" on port 80 which allows outside connectivity using Apache httpd server
(5)WordPress image "wordpress:4.8-apache" is used for launching containers and its environment variables are declared in a secret file which is not shared for security purposes
(6)MYSQL is deployed using Service Type "ClusterIP" on port 3306 which does not allow outside connectivity because MYSQL Container contains sensitive data
(7)WordPress image "mysql:5.6" is used for launching containers and its environment variables are declared in a secret file which is not shared for security purposes
