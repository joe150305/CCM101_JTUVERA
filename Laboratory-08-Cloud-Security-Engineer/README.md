# Laboratory 08 – Cloud Security Engineer

## Mission Overview

This laboratory demonstrates how to secure an Ubuntu server using UFW. An Nginx web application was deployed in a Docker container, and firewall rules were configured to control incoming traffic.

## Objectives

- Understand the Principle of Least Privilege.
- Explain the concept of an attack surface.
- Audit listening network ports.
- Apply a Default Deny incoming policy.
- Allow SSH and TCP port 8080.
- Document firewall settings and security practices.

## Commands Executed

```bash
docker --version
sudo ss -tulnp
docker run -d --name secure-web-app -p 8080:80 nginx
docker ps
curl http://localhost:8080
sudo ufw allow ssh
sudo ufw default deny incoming
sudo ufw default allow outgoing
sudo ufw enable
sudo ufw status verbose
sudo ufw allow 8080/tcp
sudo ufw status numbered
```

## Skills Learned

- Deploying an Nginx Docker container.
- Testing a web application with curl.
- Auditing listening ports on Linux.
- Configuring UFW firewall rules.
- Applying the Default Deny principle.
- Writing technical documentation in Markdown.
- Maintaining a GitHub cloud computing portfolio.

## Screenshots

The `screenshots/` directory contains terminal evidence of the running application and firewall configuration.

## Security Note

Docker-published ports may interact with firewall rules differently from ordinary host services. The actual network behavior should be verified rather than assumed.
