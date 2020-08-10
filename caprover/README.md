```
mkdir /captain && docker run -p 80:80 -p 443:443 -p 3000:3000 -v /var/run/docker.sock:/var/run/docker.sock caprover/caprover
```

For localhost

```
 -e MAIN_NODE_IP_ADDRESS='127.0.0.1'
```

```
mkdir /captain && docker run -p 80:80 -p 443:443 -p 3000:3000  -e MAIN_NODE_IP_ADDRESS='127.0.0.1' -v /var/run/docker.sock:/var/run/docker.sock caprover/caprover
```

Defualt Password : captain42



**  Automatically delete and restart all images