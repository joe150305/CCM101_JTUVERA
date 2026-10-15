# Firewall Configuration

## 1. Allow SSH

```bash
sudo ufw allow ssh
```

This allows incoming SSH connections for remote server administration.

## 2. Configure Default Policies

```bash
sudo ufw default deny incoming
sudo ufw default allow outgoing
```

Incoming connections are denied by default, while outgoing connections are allowed by default.

## 3. Enable UFW

```bash
sudo ufw enable
sudo ufw status verbose
```

These commands enable the firewall and display its status and default policies.

**Security Warning:** If `sudo ufw enable` is run before `sudo ufw allow ssh`, a remote administrator could lose SSH access because incoming SSH connections may be blocked.

## 4. Allow the Web Application

```bash
sudo ufw allow 8080/tcp
```

This adds a rule permitting TCP traffic to port 8080.

## 5. Verify the Configuration

```bash
sudo ufw status numbered
curl http://localhost:8080
```

The first command displays the numbered firewall rules. The second tests whether the web application responds locally.

## 6. Security Best Practices

- Allow only the ports required by legitimate services.
- Allow SSH before enabling the firewall.
- Use strong authentication and keep the operating system updated.
- Review firewall rules regularly.
- Check Docker's published ports and firewall behavior separately.
- Avoid exposing database services directly to the public internet.
