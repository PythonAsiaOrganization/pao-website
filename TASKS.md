# Tasks

I want to put all the data into pocketbase and run when the html build from that

## run pocketbase

```bash
docker run  \
  --name=pocketbase \
  -p 8090:8090 \
  -v ./pb_data:/pb_data \
  -v ./pb_public:/pb_public \
  --restart unless-stopped \
  ghcr.io/muchobien/pocketbase:latest
```

## create super user in docker

```bash
/usr/local/bin/pocketbase superuser upsert EMAIL PASSWORD
```

## start stopped container

```bash
docker start containerid
```

## stop container

```bash

```

## access admin pages

<http://localhost:8090/\_/>

- username : test@example.com
- password : 1234567890
