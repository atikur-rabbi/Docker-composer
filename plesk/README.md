administrator credentials: **admin** / **changeme1Q\****

```
docker run -d -p 80:80 -p 443:443 -p 8880:8880 -p 8443:8443 -p 8447:8447 plesk/plesk
```

Another way is to use automatic port mapping (publish all exposed ports to random ports with the high numbers):

```
docker run -d -P plesk/plesk
```

