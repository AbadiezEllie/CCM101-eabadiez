# Docker Compose Guide
## What Does the `services:` Block Do?
The `services:` block defines the containers that make up the application. This Compose file defines two services: `database`, which runs MariaDB 10.6, and `app`, which runs Nextcloud. Docker Compose uses these definitions to create and manage the services together.
## How Does Nextcloud Find the Database?
The `MYSQL_HOST=database` environment variable tells the Nextcloud container to connect to the database host named `database`. In Docker Compose, service names can be used as DNS names on the Compose network, so the app can reach the MariaDB service without using a hard-coded container IP address. The database credentials and database name are supplied through the other `MYSQL_*` environment variables.
## `docker run` vs. `docker-compose up -d`
`docker run` is commonly used to start an individual container and requires options such as ports and environment variables to be entered on the command line. `docker-compose up -d` reads the declarative `docker-compose.yml` file and creates or starts all services defined in it, in detached/background mode. This makes multi-container deployments easier to repeat, review, and version-control.
## Commands Used
```bash
mkdir nextcloud-deployment
cd nextcloud-deployment
nano docker-compose.yml
docker-compose up -d
docker-compose ps
docker-compose down
```
## Infrastructure as Code (IaC)
Infrastructure as Code means describing infrastructure in readable, version-controlled files instead of relying only on manual.
