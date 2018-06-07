# Nextcloud_with_docker_compose
## Prerequisites

- In order to use this compose file (docker-compose.yml) you must have:

- docker: https://docs.docker.com/install/
- docker-compose: https://docs.docker.com/compose/install/

## How to use this contents
### Clone this repository

```
git clone https://github.com/arkalira/Nextcloud_with_docker_compose
```

- Create 3 folders:

```
 mkdir -p /opt/nextcloud /opt/mysql /opt/traefik
```

- Make a copy of traefik folders content of this repo to /opt/traefik.

```
cp ./traefik/* /opt/traefik
```

- Give acme.json new permissions: 600

```
chown 600 /opt/traefik/acme.json
```

### Configuration for Nextcloud using NGINX WebProxy

### Networks name

- NETWORK=proxy

```
docker network create proxy
```

## Start your containers

```
docker-compose up --build -d
```
