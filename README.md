# tpMySQL

téléchargement de la dernière image mysql : `docker pull mysql:latest`

On run notre container : `docker run -d --name mysqlDB -p 3306:3306 -e "MYSQL_ROOT_PASSWORD=admin" mysql`

On fait un docker exec pour executé des commandes dans le container : `docker exec -it mysqlDB bash`

## Test d'une autre approche

téléchargement de la dernière image mysql et de adminer : `docker pull mysql:latest` `docker pull adminer:latest`

Installation de docker-composer si pas déjà fait : `sudo apt install docker-compose`

Création de notre fichier .yml : `stack.yml`

Docker compose de notre ficher .yml : `docker-compose -f stack.yml up`

Il suffit d'aller sur l'adresse `http://localhost:8080/` maintenant.

Une fois sur cette dernière on rentre root en user et en mot de passe celui écrit dans le ficher .yml.

On arrive alors sur l'interface de adminer.

Une fois sur adminer on peut aller dans `Privilège` afin de crée un User si besoin.

![Screenshot from 2022-01-04 16-16-40](https://user-images.githubusercontent.com/47895142/148080864-156e49b2-a07d-4b28-8d8d-e500efc65c1c.png)

ou on peut crée notre base de donnée et/ou importer toutes nos valeurs.

![Screenshot from 2022-01-04 16-20-01](https://user-images.githubusercontent.com/47895142/148081584-0960cfb6-1b4b-474c-be0e-e780257c1b45.png)

On verifie si toutes les commandes se sont bien exécutées et que les tables se sont bien créées et c'est bon.

![Screenshot from 2022-01-04 16-22-04](https://user-images.githubusercontent.com/47895142/148081936-5b9961ad-8a42-4e34-bf94-761d686507d9.png)

![Screenshot from 2022-01-04 16-24-15](https://user-images.githubusercontent.com/47895142/148082082-229233d0-258d-48bd-9a2b-78f85a7da683.png)








