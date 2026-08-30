# Cloud Infrastructure Components

## Checkpoint 3 – Understanding Cloud Infrastructure Components

This checkpoint focuses on recognizing the important resources that form a cloud infrastructure environment. Using the KillerCoda Linux Playground, I explored four major components: compute resources, storage, networking, and the operating system.

## 1. Compute Resources

**Example:** Processor (CPU) and CPU cores

**Purpose:** Compute resources are responsible for processing instructions and running programs, services, and commands.

**Importance in Cloud Computing:** They provide the computing power required by applications. Cloud providers can increase or decrease computing resources based on the workload.

**Relation to KillerCoda:** The KillerCoda Linux environment provides processor resources for running system processes and commands. Information about the CPU can be viewed using the `lscpu` and `nproc` commands.

## 2. Storage Resources

**Example:** Hard disk storage and mounted file systems

**Purpose:** Storage resources are used to keep system files, applications, user files, and other important data.

**Importance in Cloud Computing:** Cloud storage allows data to be stored and accessed when needed. Storage capacity can also be increased depending on the requirements of an application or organization.

**Relation to KillerCoda:** The Linux environment uses storage for the Ubuntu system and its files. The available and used disk space can be examined using the `df -h` command.

## 3. Networking Resources

**Example:** Network interfaces and IP addresses

**Purpose:** Networking resources enable communication between servers, users, applications, and other cloud services.

**Importance in Cloud Computing:** Networks make it possible for cloud resources to connect and exchange information. They also allow users to access applications and services through the internet.

**Relation to KillerCoda:** The KillerCoda server has network interfaces and assigned IP addresses that allow communication within the environment. Network information can be viewed using commands such as `hostname -I` or `ip addr`.

## 4. Operating System

**Example:** Ubuntu 24.04.4 LTS

**Purpose:** The operating system controls and manages the server's hardware and software resources. It also provides the platform where applications and services can operate.

**Importance in Cloud Computing:** An operating system is necessary for managing processes, memory, storage, users, and other server resources.

**Relation to KillerCoda:** KillerCoda provides an Ubuntu Linux environment where users can practice Linux commands and perform cloud computing activities.
