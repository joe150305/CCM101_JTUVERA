
# Mission Reflection

This mission helped me understand how Docker Compose can make cloud deployment easier and more organized. Instead of manually typing separate commands to create and configure every container, I can place the required configuration inside a `docker-compose.yml` file. Once the file is ready, the entire application can be deployed using the `docker-compose up -d` command. This saves time and reduces the possibility of making configuration mistakes.

I also learned that YAML is sensitive to indentation. If I use the wrong indentation or use a Tab instead of Spaces, Docker Compose may not be able to understand the configuration file correctly. This showed me that formatting is an important part of writing infrastructure configuration files.

Environment variables such as `MYSQL_PASSWORD`, `MYSQL_DATABASE`, and `MYSQL_USER` were used to provide the information needed by the MariaDB and Nextcloud containers. They allow the containers to use the required database settings without placing those settings directly into application commands.

It was interesting to see Nextcloud running after only a few deployment steps. Seeing a private cloud storage application become available through a browser helped me understand how containers can be used to deploy real applications quickly. The deployment also showed how multiple services can work together as one application.

Since Mission 1, my understanding of Cloud Computing has developed from learning basic cloud concepts to actually working with cloud infrastructure, containers, storage, and deployment tools. I now have a better understanding of how cloud engineers can use automation and Infrastructure as Code to create systems that are easier to deploy, manage, and reproduce. This mission also helped me see the importance of organization, documentation, and proper configuration when working with cloud technologies.
