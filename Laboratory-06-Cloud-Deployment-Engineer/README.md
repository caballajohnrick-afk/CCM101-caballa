# Laboratory 06 - Cloud Deployment Engineer

## Mission Overview

In this lab, I deployed a private cloud storage app using Docker Compose. The app uses two parts working together: a Nextcloud web app and a MariaDB database. I used Docker Compose to set up, run, and manage both services together as one project.

## Objectives

* Understand multi-tier application architecture.
* Create a Docker Compose YAML configuration file.
* Deploy Nextcloud and MariaDB using Docker Compose.
* Verify running containers and application access.
* Understand Infrastructure as Code (IaC).
* Document the deployment process using Markdown.

## Commands Executed

```bash
mkdir nextcloud-deployment
cd nextcloud-deployment
nano docker-compose.yml
docker-compose config
docker-compose up -d
docker-compose ps
docker-compose down
```

## Skills Learned

In this lab, I learned how to write a Docker Compose file to run multiple containers at the same time. I learned how Nextcloud talks to the MariaDB database using Docker networking and environment variables. This activity helped me better understand multi-tier apps and Infrastructure as Code.

## Screenshots

The `screenshots` folder contains evidence of the deployment, Nextcloud web interface, and container teardown.

* `compose-deployment.png`
* `nextcloud-web.png`
* `compose-teardown.png`
