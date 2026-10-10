# Multi-Tier Architecture
## What Is a Two-Tier Architecture?
A two-tier architecture separates an application into two main parts: a web/application tier and a database tier. The application tier receives requests from users and communicates with the database tier to read or save information. In this lab, Nextcloud is the application tier and MariaDB is the database tier.
## The Web/Application Tier
The web/application tier runs the Nextcloud application and presents its web interface to users. It handles HTTP requests from the browser, processes application logic, and requests database operations when it needs to read or update user and file metadata. In this deployment, the Nextcloud container exposes port 80 internally and maps it to port 8080 on the lab environment.
## The Database Tier
The database tier runs MariaDB, which stores structured information used by Nextcloud, such as user account details, configuration data, and file metadata. The database container is configured with a database name, username, and password through environment variables. The database is addressed by the Compose service name `database` from the application container.
## Why Separate the Tiers?
Separating the web application and database into different containers makes the system easier to manage, update, troubleshoot, and scale independently. It also gives each service a clearer responsibility and avoids coupling the application runtime and database software into one container. Docker Compose creates a private network so the services can communicate without exposing the database port directly to the host.
## Architecture Summary
User/browser opens the Nextcloud interface through port 8080 while Application tier in  Nextcloud receives browser requests and uses MariaDB.
The Database tier wherein MariaDB stores Nextcloud's structured application data. Latly, the Container networking is where the app connects to the database using the service name `database`.
