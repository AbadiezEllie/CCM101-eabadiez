# Cloud Storage Types Research

| Storage Type | Description | Primary Use Case | Cloud Provider Example |
|--------------|-------------|------------------|------------------------|
| **Block Storage** | Stores data in fixed-size blocks, similar to a physical hard drive. | Best for databases and low-latency workloads. | AWS EBS |
| **File Storage** | Stores data in hierarchical folders and files, like a shared drive. | Best for shared access and file systems. | AWS EFS |
| **Object Storage** | Stores data as objects with metadata and unique identifiers. | Best for unstructured data such as images, videos, and backups. | AWS S3 |

### Why Object Storage?
Object Storage is the best choice for storing millions of user-uploaded images because it is highly scalable, supports metadata for easy organization, and is accessible via APIs. 
