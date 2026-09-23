# MinIO Object Storage Deployment

## Deployment Overview

For this laboratory activity, I deployed MinIO using Docker on an Ubuntu environment provided by KillerCoda. MinIO was used as an S3-compatible object storage server for storing user-uploaded files.

## Docker Command

The following Docker command was used to deploy the MinIO server:

```bash
docker run -d -p 9000:9000 -p 9001:9001 --name minio-server \
-e "MINIO_ROOT_USER=cloudadmin" \
-e "MINIO_ROOT_PASSWORD=CloudNova2026!" \
quay.io/minio/minio server /data --console-address ":9001"
