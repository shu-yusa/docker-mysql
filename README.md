# README
MySQL server by docker.


## Prerequisites
Docker has to be installed. ([Install Docker for Mac](https://docs.docker.com/docker-for-mac/install/))

## Create and launch container
```bash
docker-compose up
```
`Ctrl-C` to stop the container.

To daemonize container,
```bash
docker-compose up -d
```

To stop container,
```bash
docker-compose down
```

## Connecting to the MySQL server
To login the container,
```bash
docker exec -it docker-mysql bash
```

To directly connect to the MySQL,
```bash
mysql -u `user_name` -h 127.0.0.1 -p
```
and enter password.

## Configuration
The root password, database name, user name, and the user's password can be set in docker-compose.yml.
