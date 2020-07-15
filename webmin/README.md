
docker start webmin
sudo docker stop webmin
sudo docker rm webmin
sudo docker rmi tragus/webmin 


sudo docker run -d -p 10000:10000 --name webmin jgrojasx/webmin

sudo docker stop webmin
sudo docker rm webmin
sudo docker run -d -p 10000:10000 --restart unless-stopped --name webmin jgrojasx/webmin

username: root
password: admin

install apache
install php-mysql


for vertualmin

sudo docker run-p 10000:10000 --name=hosting \
-v hosting-etc:/etc \
-v hosting-home:/home \
-v hosting-lib:/var/lib \
-v hosting-log:/var/log \
-v hosting-www:/var/www \
--hostname=server.virtualmin.host --net=host \
--privileged --restart unless-stopped -d technoexpress/virtualmin


