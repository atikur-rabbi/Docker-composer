sudo docker run -d -p 8080:80 nextcloud

sudo docker run --rm -d -p 8080:80 --name nextcloud nextcloud

sudo docker run --restart unless-stopped -d -p 8011:80 --name nextcloud nextcloud



