# Laboratory 06 - Cloud Deployment Engineer

## Mission Overview

This laboratory focused on deploying a multi-tier private cloud storage application using Docker Compose. The application consisted of a Nextcloud web application and a MariaDB database. Docker Compose was used to define and deploy both services as a single application stack.

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

Through this mission, I learned how to create a Docker Compose configuration and use it to deploy multiple containers together. I also learned how a Nextcloud application communicates with a MariaDB database through Docker Compose networking and environment variables. The activity improved my understanding of multi-tier architecture and Infrastructure as Code.

## Screenshots

The `screenshots` folder contains evidence of the deployment, Nextcloud web interface, and container teardown.

* `compose-deployment.png`
* `nextcloud-web.png`
* `compose-teardown.png`
