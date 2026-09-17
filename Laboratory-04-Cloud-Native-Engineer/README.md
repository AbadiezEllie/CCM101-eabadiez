# Laboratory 04 - Cloud-Native Engineer

## Mission Overview
This mission focuses on transitioning from traditional virtualization to containerization. As a Cloud-Native Engineer, I explored Docker, deployed a containerized Nginx web server, and documented the container lifecycle.

## Objectives
- Differentiate between Virtual Machines (VMs) and Containers.
- Access a Docker-enabled environment using KillerCoda.
- Execute fundamental Docker CLI commands.
- Deploy and manage a containerized Nginx application.
- Document technical procedures in Markdown.
- Continue building a professional GitHub Cloud Computing Portfolio.

## Docker Commands Executed
- `docker --version`
- `docker info`
- `docker pull nginx`
- `docker run -d -p 8080:80 --name mynginx nginx`
- `curl http://localhost:8080`
- `docker ps`
- `docker stop mynginx`
- `docker rm mynginx`

## Skills Learned
- Understanding differences between VMs and containers.
- Running and managing Docker containers.
- Port mapping for containerized applications.
- Writing structured technical documentation in Markdown.

## Challenges Encountered
- Initial unfamiliarity with Docker CLI syntax.
- Ensuring proper port mapping for Nginx accessibility.
- Remembering to stop and remove containers to avoid resource conflicts.
