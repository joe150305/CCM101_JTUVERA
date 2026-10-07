
# Laboratory 07 – Cloud Operations Engineer

## Mission Overview

This laboratory focuses on cloud operations, observability, monitoring, application logging, and container performance. The activity uses a Linux server and Docker to monitor system resources, deploy an Nginx web server, generate web traffic, analyze application logs, and monitor container resource usage.

## Objectives

- Monitor Linux CPU, memory, and disk resources.
- Establish a baseline for the host system.
- Deploy an Nginx web server using Docker.
- Generate HTTP requests and errors.
- Analyze Docker application logs.
- Monitor real-time container resource usage.
- Document cloud operations findings using Markdown.

## Monitoring Commands Executed

The following commands were used during the laboratory:

```bash
free -h
df -h
top
docker run -d --name client-website -p 8080:80 nginx
curl http://localhost:8080
curl http://localhost:8080
curl http://localhost:8080
curl http://localhost:8080/hidden-admin-page
docker logs client-website
docker stats
