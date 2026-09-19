
# Docker Deployment

## Mission 4: The Cloud-Native Engineer

This document logs the execution of Docker commands during Laboratory 04 within the KillerCoda Ubuntu environment. The activity demonstrates a standard containerized application workflow, covering engine verification, image retrieval, Nginx web server deployment, service testing, and container lifecycle management.

Rather than installing Nginx directly on the host operating system, it was deployed as an isolated Docker container. This highlights key cloud-native advantages, such as application portability, environment consistency, and lightweight execution.

---

# Checkpoint 3: Enter the Docker Playground

## Environment Setup

All laboratory tasks were executed inside the interactive KillerCoda Ubuntu Playground, which provides a pre-configured Ubuntu Linux environment with Docker pre-installed.

The primary objective of this checkpoint was to validate that the Docker Engine daemon and CLI were fully operational prior to container deployment.

---

## 1. Verify Installed Docker Version

To confirm that Docker is installed and accessible via the terminal, execute the following command:

```bash
docker --version
