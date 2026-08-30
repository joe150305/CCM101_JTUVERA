# Mission Overview

This laboratory activity is about exploring the structure and important parts of a cloud computing environment. Through the KillerCoda Linux Playground, I examined a Linux-based server and gathered information about its processor, memory, storage, network, and operating system.

The activity also involved studying similar cloud services offered by Amazon Web Services (AWS), Microsoft Azure, and Google Cloud Platform (GCP). I also developed a simple infrastructure design and documented my work in my GitHub Cloud Computing Portfolio.

## Objectives

- Learn about the essential parts of a cloud environment.
- Explore a Linux server using command-line tools.
- Examine the server's computing, storage, network, and system resources.
- Understand the relationship between different cloud infrastructure components.
- Identify similar services provided by AWS, Azure, and GCP.
- Develop a simple cloud infrastructure design.
- Practice creating technical documentation using Markdown.
- Organize laboratory outputs in a GitHub repository.

## Cloud Infrastructure Components

### Compute Resources

Compute resources handle the processing of programs and workloads. The Linux environment used in this activity runs on an **Intel Xeon E312xx processor with 1 CPU core**.

### Storage Resources

Storage resources are responsible for keeping operating system files, applications, and other data. The server contains a **19 GB root storage disk** along with other mounted file systems.

### Networking Resources

Networking makes communication possible between the cloud server and other devices or systems. The KillerCoda environment includes network addresses such as `172.30.1.2` and `172.17.0.1`.

### Operating System

The operating system controls the server's hardware and provides the environment needed to run applications. The system used for this activity is **Ubuntu 24.04.4 LTS**, running on the **6.8.0-138-generic kernel**.

## Tools and Technologies Used

- KillerCoda Linux Playground
- Ubuntu Terminal
- GitHub
- Git
- Markdown
- Draw.io
- Web Browser

## Linux Commands Used

```bash
cat /etc/os-release
uname -r
lscpu
nproc
free -h
lsblk
df -h
mount | column -t
hostname
hostname -I
ip addr
