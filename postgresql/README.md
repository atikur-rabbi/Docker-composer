
## 1. Create a folder in a known location for you
```
$ mkdir ${HOME}/postgres-data/
```
## 2. run the postgres image
```
$ docker run -d \
	--name dev-postgres \
	-e POSTGRES_PASSWORD=Pass2020! \
	-v ${HOME}/postgres-data/:/var/lib/postgresql/data \
        -p 5432:5432 \
        postgres
```
## 3. check that the container is running
```
$ docker ps
>>>
CONTAINER ID        IMAGE               COMMAND                  CREATED             STATUS              PORTS                    NAMES
dfa570d6e843        postgres            "docker-entrypoint.s…"   27 hours ago        Up 3 seconds        0.0.0.0:5432->5432/tcp   postgres-test
```



# Starting the pgAdmin instance

```
$ docker pull dpage/pgadmin4
$ docker run \ 
    -p 80:80 \
    -e 'PGADMIN_DEFAULT_EMAIL=user@domain.local' \
    -e 'PGADMIN_DEFAULT_PASSWORD=SuperSecret' \
    --name dev-pgadmin \ 
    -d dpage/pgadmin4
```

docker run  -p 80:80  -e 'PGADMIN_DEFAULT_EMAIL=user@domain.local'   -e 'PGADMIN_DEFAULT_PASSWORD=SuperSecret'  --name dev-pgadmin  -d dpage/pgadmin4



docker run -d --name dev-postgres -e POSTGRES_PASSWORD=Pass2020 -p 5432:5432 postgres

docker run -d --name postgres -e POSTGRES_PASSWORD=postgres  -p 5432:5432 postgres



docker run -p 8080:8080 --link postgres:postgres eswork/pgweb

docker build -p 8080:8080 --link postgres:postgres eswork/pgweb