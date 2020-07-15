Ajenti Install

```
sudo docker run --restart unless-stopped -p 80:80 -p 443:443 -p 8002:8000 -p 8001:8001 -v /opt/ajenticp/ajenti:/ajenti -v /opt/ajenticp/backup:/backup -d niiknow/ajenticp
```

