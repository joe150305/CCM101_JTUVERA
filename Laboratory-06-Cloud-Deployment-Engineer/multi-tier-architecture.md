
---

### `multi-tier-architecture.md`

```markdown
# Multi-Tier Architecture

## What is a Two-Tier Architecture?

A two-tier architecture is a system that separates an application into two main layers: the application tier and the database tier. In this laboratory activity, Nextcloud serves as the application tier while MariaDB serves as the database tier.

## The Web/Application Tier

The web or application tier is responsible for providing the user interface and handling requests from users. In this activity, the Nextcloud container provides the web application that users access through a browser.

The Nextcloud application runs inside its own Docker container and communicates with the MariaDB database to store and retrieve information.

## The Database Tier

The database tier is responsible for storing persistent application data. In this activity, MariaDB is used as the database system for Nextcloud.

The MariaDB container stores information such as user accounts, database records, and other metadata required by the Nextcloud application.

## Why Separate Them?

Separating the web application and database into different containers makes the system easier to manage and maintain. Each container can have its own purpose, configuration, and resources.

This separation also allows the application and database to be updated, restarted, or scaled independently without placing both components inside a single container.
