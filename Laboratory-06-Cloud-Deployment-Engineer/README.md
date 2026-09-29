# Laboratory 06 - Cloud Deployment Engineer

## Mission Overview

This laboratory activity focuses on deploying a multi-tier private cloud storage application using Docker Compose. The application consists of a Nextcloud web application and a MariaDB database running in separate containers. Docker Compose allows both containers to be configured and deployed together using a single YAML configuration file.

## Objectives

- Explain the concept of a multi-tier application architecture.
- Understand the purpose and structure of a `docker-compose.yml` file.
- Use the Linux command-line text editor `nano` to create configuration files.
- Deploy a multi-container application using Docker Compose.
- Understand Infrastructure as Code (IaC).
- Document the deployment process using Markdown.
- Expand the Cloud Computing GitHub portfolio.

## Commands Executed

The following commands were used during the laboratory activity:

```bash
mkdir nextcloud-deployment
cd nextcloud-deployment
nano docker-compose.yml
docker-compose up -d
docker-compose ps
docker-compose down
