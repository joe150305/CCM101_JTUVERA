
# Mission Reflection

This laboratory activity helped me understand why monitoring is an important responsibility of a Cloud Operations Engineer. I learned that deploying an application is not enough because the server and application must also be monitored to ensure reliable performance.

First, checking host resources is important even when containers are running perfectly. Containers depend on the host server's CPU, memory, and disk storage. If the host runs out of resources, applications may become slow, stop responding, or crash. Checking the system baseline helps engineers identify possible problems before they affect users.

Second, the `docker logs` command helps troubleshoot login problems by showing application messages and errors. An engineer can examine the logs to identify failed requests, authentication errors, or other problems recorded by the application. However, additional investigation may be necessary if the application does not log the specific cause.

Third, logs and metrics provide different types of information. Logs record individual events, requests, and errors, while metrics show numerical measurements such as CPU usage, memory consumption, and network traffic. Using both allows engineers to understand what happened and evaluate how the system was performing at that time.

Large enterprise companies can monitor thousands of containers using centralized monitoring platforms. Tools such as Prometheus collect and store metrics, while Grafana displays those metrics through dashboards and visualizations. Alerting systems can notify engineers when resource usage exceeds established limits or applications become unhealthy.

Finally, this activity improved my ability to troubleshoot Linux environments by teaching me how to inspect system resources, deploy a web server, generate HTTP requests, examine application logs, and monitor Docker containers. I also learned the importance of recording actual results and supporting technical reports with screenshots.

Overall, I gained a better understanding of observability and how monitoring tools help engineers maintain application reliability. These skills will be useful in managing cloud infrastructure and diagnosing problems in real-world IT environments.
