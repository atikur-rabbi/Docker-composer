Install collabora office

```
sudo docker run -t -d -p 9980:9980 -e "extra_params=--o:ssl.enable=false" collabora/code
```

go to 

http://192.168.100.20:9980