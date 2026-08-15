# CCM101 Cloud Computing

## Laboratory Activity 1 – Mission 1: Introduction to the Cloud

### Mission Overview

This laboratory activity covers the fundamental skills required for working with cloud infrastructure. It involves using a Linux environment, navigating and managing files and directories, checking system information, and building a professional GitHub portfolio.

---

## Mission Objectives

- Access an online Linux environment through KillerCoda.
- Learn how to navigate and use the Linux operating system.
- Collect essential system information.
- Manage and organize files and directories using Linux commands.
- Set up and manage a GitHub repository.
- Record and present technical work using Markdown.

---

# Checkpoint 1 – Accessing the Cloud

For this checkpoint, I started an Ubuntu Linux Playground through KillerCoda. I created a Linux user named **jtuvera**, configured a Bash shell and home directory, and provided the user with sudo privileges.

### User Information

| Information | Result |
|---|---|
| Current Username | jtuvera |
| Current Working Directory | /home/jtuvera |
| Hostname | `[Your Hostname]` |

### Commands Used

```bash
sudo adduser jtuvera
sudo usermod -aG sudo jtuvera
su - jtuvera

whoami
pwd
hostname
