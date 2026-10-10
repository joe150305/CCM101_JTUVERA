# Laboratory Activity 7: The Cloud Operations Engineer

## Mission Overview

This laboratory activity focuses on monitoring a Linux host and observing the performance of a containerized web server. Using KillerCoda and Docker, I checked system resources, deployed Nginx, generated HTTP requests, examined application logs, and monitored container metrics.

## Objectives

- Check host memory and disk capacity.
- Observe CPU usage and running processes.
- Deploy an Nginx container.
- Generate successful and failed HTTP requests.
- Analyze Docker application logs.
- Monitor container CPU, memory, and network usage.
- Document results using Markdown.

## Monitoring Commands Executed

| Command | Purpose |
|---|---|
| `free -h` | Check memory usage |
| `df -h /` | Check root filesystem capacity |
| `top` | Monitor CPU and running processes |
| `docker ps` | View running containers |
| `docker run -d --name client-website -p 8080:80 nginx` | Deploy Nginx |
| `curl -i http://localhost:8080` | Test successful HTTP requests |
| `curl -i http://localhost:8080/hidden-admin-page` | Generate an HTTP 404 response |
| `docker logs client-website` | View application logs |
| `docker stats` | Monitor container resource usage |

## Skills Learned

- Linux system monitoring
- Docker container deployment
- HTTP request testing
- Application log analysis
- Real-time resource monitoring
- Technical documentation using Markdown
- GitHub portfolio management

## Evidence

Screenshots of the terminal outputs are stored in the `screenshots/` folder.

## Conclusion

This activity demonstrated how Linux commands and Docker tools help engineers monitor server health, troubleshoot web application errors, and evaluate container resource consumption.
