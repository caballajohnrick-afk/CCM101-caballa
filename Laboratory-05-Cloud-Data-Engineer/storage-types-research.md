# Cloud Storage Types Research

## Storage Types Comparison

| Storage Type | Description | Primary Use Case | Cloud Provider Example |
| :--- | :--- | :--- | :--- |
| **Block Storage** | Splitting data into fixed-size blocks, each with a unique address, acting like an unformatted hard drive. | Databases, Operating System volumes, high-performance applications. | AWS EBS (Elastic Block Store) |
| **File Storage** | Storing data in a hierarchical file system with folders and subfolders accessible over a network. | Shared network drives, legacy applications, content management systems. | AWS EFS (Elastic File System) |
| **Object Storage** | Storing data as distinct units (objects) containing raw data, metadata, and a unique identifier in a flat namespace. | Unstructured data storage (images, videos, backups, big data analytics). | AWS S3 (Simple Storage Service) |

## Client Explanation

Object Storage is the ideal choice for storing your user-uploaded images because it is designed to handle massive amounts of unstructured data efficiently without file system overhead. Unlike block or file storage, object storage scales infinitely at a lower cost and allows rich custom metadata to be attached to each image. Furthermore, it decouples media assets from the web server instances, ensuring performance remain fast and reliable as your user base grows.
