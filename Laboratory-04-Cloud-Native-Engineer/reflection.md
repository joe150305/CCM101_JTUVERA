# Mission Reflection

This laboratory activity helped me understand how Docker containers can make application deployment faster and more efficient. A Docker container can start within seconds because it does not need to boot an entire operating system. In comparison, a Virtual Machine needs to start a complete Guest Operating System, which takes more time and uses more resources. Docker provides a lightweight approach for running applications and their dependencies.

Port mapping is necessary because the web server is running inside the isolated network environment of the container. The command `-p 8080:80` connects port 8080 on the host machine to port 80 inside the Nginx container. This allows me to access the Nginx web server through `http://localhost:8080`. Without port mapping, the web server would not be directly accessible through the host's port 8080.

When the `docker rm` command is used, the container is permanently removed from the Docker environment. Data stored only inside the container's writable layer is also deleted when the container is removed. However, data stored using Docker volumes can remain available even after the container is deleted.

Containerization can improve collaboration between software developers and IT operations teams. Developers can package applications together with their required dependencies inside containers. Operations teams can then deploy the same container in different environments, helping reduce differences between development, testing, and production. This supports DevOps practices such as automation, consistency, and faster deployment.

My GitHub portfolio is also evolving as I continue adding laboratory activities and technical documentation. Lab 4 adds practical experience with Docker, Nginx, Linux commands, and container management. Keeping my files, documentation, and screenshots organized in GitHub gives me a record of my progress and the technical skills I am developing in cloud computing.
