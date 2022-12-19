# Wordpress in Docker

Serve a WordPress instance running in Docker on your server. 

## Prerequisites
- Docker installed on server
- A traefik reverse proxy is already running in Docker that is connected to the Docker network `traefik-net`. 
- A subdomain pointing to your server

## Start Services

Replace passwords and subdomain in `docker-compose.yml`. Then run following command:

```shell
docker-compose up -d
```

> After first start, a setup page is served. Visit your domain and create your initial WordPress user and website.


## Stop Services

```shell
docker-compose down
```