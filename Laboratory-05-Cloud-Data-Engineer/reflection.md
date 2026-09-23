
# Mission Reflection

This laboratory activity helped me understand why object storage is suitable for applications that need to store millions of photos. Object storage is designed for large amounts of unstructured data such as images, videos, documents, and backups. Instead of treating each file like a traditional hard drive block, object storage stores data as objects with metadata and unique identifiers. This makes it practical for a photo-sharing application where users can continuously upload large numbers of images.

Docker made the deployment of MinIO easier because I did not need to manually install and configure all of the required components. I used a Docker command to download the MinIO image, create the container, configure the administrator credentials, and expose the required ports. When the original `minio/minio` image could not be pulled, I used the `quay.io/minio/minio` image instead. This experience showed me how Docker can make cloud service deployment faster and more consistent.

A bucket is a container used by object storage to organize and store objects. In this activity, I created a bucket named `client-photos`. I then uploaded a test file inside the bucket to demonstrate that the MinIO object storage server was working correctly.

Large enterprise companies can protect object storage data from physical server failures by using redundancy, replication, backups, and distributed storage systems. They can keep multiple copies of data across different storage devices or locations. These methods help prevent data loss when hardware fails.

My confidence in using the Linux command line is also improving. I became more comfortable entering Docker commands, checking running containers with `docker ps`, and verifying the deployment. I also learned that understanding command options is important because each option controls part of the container configuration. Overall, this mission gave me practical experience with Linux, Docker, MinIO, object storage, and cloud infrastructure.
