### Shopware 6 Setup

#### Bind-Mounting Setup
- exlude volumes from docker-compose.yml
- ``` docker compose down ```
- ``` docker compose up -d ```
- ``` mkdir src ```
- ``` sudo chgrp -R 33 ./src ```
- ``` sudo chmod a+w ./src/var/* ```
- ``` sudo docker cp <container_name>:/var/www/html/. <path/to/src/folder> ```
- ``` docker compose stop ```
- ``` docker compose up -d ```
- ``` docker exec -it <container_name> bash ```
- ``` sudo chown www-data:www-data /var/www/html -R```
- ``` bin/console theme:change ```
- ``` bin/console theme:compile ```
