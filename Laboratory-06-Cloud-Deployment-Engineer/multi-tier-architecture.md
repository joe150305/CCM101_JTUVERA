
# Multi-Tier Architecture

## What is a Two-Tier Architecture?

A two-tier architecture is a system divided into two main parts: the application or web tier and the database tier. In this laboratory activity, Nextcloud serves as the web/application tier while MariaDB serves as the database tier.

## The Web/Application Tier

The web/application tier is responsible for providing the user interface and handling requests from users. In this activity, the Nextcloud container runs the web application and allows users to access the private cloud storage system through a web browser.

The Nextcloud application communicates with the MariaDB database to store and retrieve information required by the application.

## The Database Tier

The database tier is responsible for storing persistent information used by the application. MariaDB is used in this activity to store Nextcloud data such as user accounts, configuration information, and file metadata.

The database runs in its own Docker container and communicates with the Nextcloud application container.

## Why Separate Them?

Separating the web application and database into different containers makes the system easier to manage and maintain. Each container has a specific responsibility, and one component can be updated or restarted without placing both application and database services in the same container.
