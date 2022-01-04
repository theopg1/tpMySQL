# tpMySQL

téléchargement de la dernière image mysql : `docker pull mysql:latest`

On run notre container : `docker run -d --name mysqlDB -p 3306:3306 -e "MYSQL_ROOT_PASSWORD=admin" mysql`

On fait un docker exec pour executé des commandes dans le container : `docker exec -it mysqlDB bash`
