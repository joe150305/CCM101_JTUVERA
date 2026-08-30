# Infrastructure Report

## Checkpoint 2 – Examining the Cloud Server

### Overview

This report contains the information collected from the Linux cloud server in the KillerCoda Playground. Several Linux commands were executed to examine the server's operating system, processor, memory, disk space, network configuration, and other important system details.

The purpose of this investigation is to better understand the resources available in a cloud-based Linux environment and how these resources support applications and services.

## 1. Operating System

**Command used:**

`cat /etc/os-release`

**Result:**

The cloud server is running **Ubuntu 24.04.4 LTS**, also known by the codename **Noble Numbat**.

The operating system manages the hardware and software resources of the server and provides the environment needed for Linux applications and services to operate.

## 2. Kernel Version

**Command used:**

`uname -r`

**Result:**

The Linux kernel version is:

`6.8.0-138-generic`

The kernel is an important part of the operating system because it manages communication between the software and the hardware resources of the server.

## 3. CPU Model

**Command used:**

`lscpu | grep "Model name"`

**Result:**

The server uses:

**Intel Xeon E312xx (Sandy Bridge, IBRS update)**

The processor provides the computing power needed to execute Linux commands, system processes, applications, and other workloads running in the cloud environment.

## 4. CPU Cores

**Command used:**

`nproc`

**Result:**

The server has **1 available CPU core**.

The CPU core is responsible for processing instructions and performing computing tasks. In this KillerCoda environment, the available core provides the processing resources needed for the Linux activities performed during the laboratory exercise.

## 5. Total RAM

**Command used:**

`free -h`

**Result:**

The server has approximately **1.9 GiB of RAM**.

The memory information gathered from the server is listed below:

- **Total Memory:** 1.9 GiB
- **Used Memory:** 421 MiB
- **Free Memory:** 852 MiB
- **Available Memory:** 1.4 GiB
- **Swap Space:** 1.0 GiB

RAM is used by the operating system and running applications to temporarily store information while processes are active. Available memory is important because applications and services need memory to run properly.

The server also has swap space, which can be used as additional virtual memory when needed.

## 6. Disk Capacity

**Command used:**

`df -h`

**Result:**

The main storage device, `/dev/vda1`, provides approximately **19 GB** of disk space.

The storage information is shown below:

| File System | Size | Used | Available | Use | Mounted On |
|---|---:|---:|---:|---:|---|
| `/dev/vda1` | 19G | 5.4G | 13G | 30% | `/` |
| `/dev/vda16` | 881M | 117M | 117M | 15% | `/boot` |
| `/dev/vda15` | 105M | 6.2M | 99M | 6% | `/boot/efi` |

The main root file system `/` contains important operating system files, applications, and other system data.

The `/boot` partition stores files required during the system startup process, while `/boot/efi` contains files related to the EFI boot system.

Storage is an important part of cloud infrastructure because it provides space for operating systems, applications, files, and other data.

## 7. Mounted File Systems

**Command used:**

`mount | column -t`

**Result:**

The server contains multiple mounted file systems, including:

- `/`
- `/boot`
- `/boot/efi`
- `/run`
- `/dev/shm`
- `/proc`
- `/sys`
- `/dev`

These mounted locations support different functions of the Linux operating system.

The root directory `/` is the primary file system used by the server. The `/boot` and `/boot/efi` locations contain files needed during startup.

Other file systems such as `/proc` and `/sys` provide information about system processes, the kernel, and hardware resources. The `/dev` directory provides access to devices, while `/run` and `/dev/shm` are used for runtime and temporary system information.

Together, these mounted file systems help the Linux operating system organize and manage its resources.

## 8. Hostname

**Command used:**

`hostname`

**Result:**

The server hostname is:

**ubuntu**

A hostname is used to identify a computer or server within a system or network environment. It helps distinguish the server from other devices and resources.

In this KillerCoda cloud environment, the server is identified by the hostname **ubuntu**.

## 9. IP Address

**Command used:**

`hostname -I`

**Result:**

The server has the following IP addresses:

`172.30.1.2 172.17.0.1`

These IP addresses allow the server to communicate within its network and cloud environment.

IP addresses are important networking resources because they identify devices and allow communication between servers, applications, and other network resources.

## Summary

Based on the investigation, the KillerCoda Linux cloud environment is running **Ubuntu 24.04.4 LTS (Noble Numbat)** with the **6.8.0-138-generic** Linux kernel.

The server uses an **Intel Xeon E312xx (Sandy Bridge, IBRS update)** processor and provides **1 CPU core** for processing workloads. It also has approximately **1.9 GiB of RAM** and **1.0 GiB of swap space**.

For storage, the main disk `/dev/vda1` provides approximately **19 GB** of capacity. The server also uses several mounted file systems to support different Linux functions and system operations.

The hostname of the server is **ubuntu**, and its identified IP addresses are `172.30.1.2` and `172.17.0.1`.

Overall, the server provides the essential resources required for a Linux cloud environment. These include **compute resources for processing**, **memory for active processes**, **storage for files and applications**, and **networking for communication**.

## Overall Observation

The investigation demonstrates that a cloud server depends on several infrastructure components working together.

The **CPU** provides the processing capability needed to execute commands and applications. **RAM** supports running processes by providing temporary memory. **Storage** keeps the operating system, applications, and files. **Networking** allows the server to communicate with other systems and services.

The **Ubuntu operating system** manages all of these resources and provides a platform where applications and services can run.

Using Linux commands such as `lscpu`, `nproc`, `free -h`, `df -h`, `hostname`, and `hostname -I` made it possible to examine the actual configuration of the server.

## Evidence

Screenshots showing the Linux commands and their corresponding results are saved in the `screenshots` folder of this GitHub repository.

### Screenshot 1

This screenshot shows the following system information:

- Operating system details
- Linux kernel version
- CPU model
- Number of CPU cores
- RAM information
- Disk capacity
- Mounted file systems

### Screenshot 2

This screenshot contains additional information about the server, including:

- Additional mounted file systems
- Server hostname
- IP addresses
- Network-related information

These screenshots serve as evidence of the commands executed and the information collected from the KillerCoda Linux cloud environment.
