# Docker Compose Guide

## What does the `services:` block do?

The services: block lists the containers used in this app. For this project, it includes two services: database for MariaDB and app for Nextcloud. Docker Compose uses these settings to build and run both containers.

## How does the Nextcloud app find the database?

The Nextcloud app uses the `MYSQL_HOST` environment variable to identify the database service. In the Compose file, it is set to `database`, which matches the name of the MariaDB service:

```yaml
- MYSQL_HOST=database
```

Docker Compose creates a network for the services, allowing the Nextcloud container to communicate with the MariaDB container using the service name `database`.

## Difference Between `docker run` and `docker-compose up -d`

docker run is used to start one container at a time using command-line commands, like running a single Nginx web server. In contrast, docker-compose up -d starts multiple related containers defined in a Compose YAML file. In this lab, one command starts both Nextcloud and MariaDB together. The -d flag runs them in the background so you can keep using the terminal.

## Infrastructure as Code

Docker Compose demonstrates Infrastructure as Code because the application infrastructure is described in a YAML configuration file. Instead of manually entering many commands, the configuration can be reused to consistently deploy the same multi-container environment.

