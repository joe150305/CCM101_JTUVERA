# Security Audit Report

## 1. Principle of Least Privilege (PoLP)

The Principle of Least Privilege means giving users and applications only the permissions they need to perform their tasks. In cloud environments, this reduces the damage that can occur if an account or service is compromised.

## 2. Attack Surface

An attack surface is the collection of entry points that an attacker could use to access or exploit a virtual machine. Open network ports, running services, weak passwords, and unnecessary software can increase the attack surface.

## 3. Default Deny Policy

A Default Deny policy blocks incoming traffic unless a firewall rule explicitly allows it. This is safer than trying to block individual attackers because unknown or unauthorized connections are also restricted by default.

## 4. Server Audit

**Environment:** KillerCoda Ubuntu Playground

**Application:** Nginx Docker container named `secure-web-app`

**Application Port:** TCP 8080

**Audit Command:**

```bash
sudo ss -tulnp
```

This command lists listening TCP and UDP sockets and associated processes when sufficient permissions are available.

**Observed Results:**

Record the ports and services actually shown by your terminal. Do not assume that every port is open.

## 5. Security Findings

- The web application was deployed and tested using curl.
- UFW was configured with a default-deny incoming policy.
- Outgoing traffic was allowed by default.
- SSH and TCP port 8080 were explicitly allowed.
- The final firewall status was checked using `sudo ufw status numbered`.

**Conclusion:** The mission demonstrates how firewall rules can restrict network access. Docker-published ports should also be checked because Docker networking rules can affect how UFW filters traffic.
