# Laboratory 04: The Cloud-Native Engineer

## Executive Summary

Laboratory 04 explores cloud-native engineering principles, focusing on containerization and container management with Docker. The primary goal of this activity is to analyze the architectural and operational differences between traditional Virtual Machines (VMs) and lightweight Linux containers, while executing a core Docker workflow within an interactive KillerCoda environment.

During this lab, the KillerCoda Playground was utilized to verify Docker installation, pull the official Nginx container image, instantiate and run an Nginx web server, map host-to-container ports, issue HTTP test requests, and manage the complete container lifecycle. All steps and output verification have been documented in Markdown and archived in the GitHub Cloud Computing portfolio.

---

## Objectives

* **Architectural Analysis & Comparison:**
  * Compare Virtual Machines and Containers across boot speed, resource consumption, overhead, and isolation boundaries.
  * Contrast hypervisor-based virtualization (Hardware-level) with containerization (OS-level virtualization).
* **Hands-on Docker Operations:**
  * Provision a Docker-enabled environment on KillerCoda Ubuntu.
  * Validate system environment and Docker daemon status via CLI.
  * Pull official container images from Docker Hub (`nginx`).
  * Launch containers in detached mode (`-d`) with host port forwarding (`-p 8080:80`).
  * Verify HTTP service availability locally using `curl`.
  * Execute container lifecycle management (listing, stopping, and removing container instances).
* **Documentation & Portfolio Integration:**
  * Document command execution sequences and terminal outputs using structured Markdown.
  * Version-control lab artifacts and screenshot evidence within GitHub.

---

## Environment Specifications

All Docker operations were executed using the KillerCoda Ubuntu Playground environment:

| Property | Value |
| :--- | :--- |
| **Operating System** | Ubuntu 24.04.4 LTS |
| **System Architecture** | x86_64 |
| **Docker Engine Version** | 29.1.3 |

---

## Command Execution & Verification

### Checkpoint 3: Docker Engine Verification

#### 1. Verify Installed Docker Version

To confirm that the Docker Engine CLI and runtime daemon are properly installed and accessible, run:

```bash
docker --version
