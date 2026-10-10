# Mission 6: The Cloud Deployment Engineer
## Mission Overview
This laboratory deploys a two-tier private cloud storage proof of concept using Nextcloud as the web/application tier and MariaDB as the database tier. Docker Compose defines both services in a YAML file and deploys them together.
## Objectives- Explain a two-tier application architecture.- Create and understand a `docker-compose.yml` file.- Deploy and inspect a multi-container application with Docker Compose.- Access the Nextcloud setup page through port 8080.- Document Infrastructure as Code principles in Markdown.- Capture evidence and maintain the GitHub Cloud Computing Portfolio.
## Commands Executed
```bash
mkdir nextcloud-deployment
cd nextcloud-deployment
nano docker-compose.yml
docker-compose up -d
docker-compose ps
docker-compose down
```
## Skills Learned- Linux command-line navigation and editing with nano.- YAML syntax and indentation.- Docker Compose service definitions and multi-container deployment.- Container-to-container communication using service names.- Accessing a containerized web application through a published port.- Markdown technical documentation, Git commits, and GitHub portfolio maintenance.


