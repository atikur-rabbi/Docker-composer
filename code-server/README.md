Samples

docker run -it -p 127.0.0.1:8080:8080 \
  -v "$PWD:/home/coder/project" \
  -u "$(id -u):$(id -g)" \
  codercom/code-server:latest


 sudo docker run -it -p 8080:8080 \
  -v "$PWD:/home/coder/project" \
  -u "$(id -u):$(id -g)" \
  codercom/code-server:latest


sudo docker run -it -p 8080:8080 -e PASSWORD='yourpassword' -v "${PWD}:/home/coder/project" codercom/code-server 