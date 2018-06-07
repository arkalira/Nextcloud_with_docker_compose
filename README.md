# Nextcloud_with_docker_compose

## Prerequisites
In order to use this compose file (docker-compose.yml) you must have:

- docker: https://docs.docker.com/install/
- docker-compose: https://docs.docker.com/compose/install/

## How to use
### Clone this repository

```
git clone https://github.com/arkalira/Nextcloud_with_docker_compose
```

- Make a copy of our .env.sample and rename it to .env:
- Update this file with your preferences.

### Configuration for Nextcloud using NGINX WebProxy

```
### Networks name

** Your container app must use a network conencted to your webproxy **
 - https://github.com/evertramos/docker-compose-letsencrypt-nginx-proxy-companion

- NETWORK=frontend
- NETWORK=backend

## Start your container

```
$ docker-compose up -d
```
