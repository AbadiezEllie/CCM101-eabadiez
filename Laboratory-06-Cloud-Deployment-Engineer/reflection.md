# Mission 6: Mission Reflection

Writing a `docker-compose.yml` file makes a cloud engineer's job easier because it allows multiple containers to be configured and deployed using a single file. Instead of manually typing commands for each container, Docker Compose lets me define the services, ports, and environment variables in one place. This makes deployment faster, more organized, and easier to repeat.

If I make an indentation error in a YAML file, such as using a Tab instead of spaces, Docker Compose may fail to read the configuration correctly. It can display an error message and prevent the containers from starting. This taught me to be careful with indentation and to check my code before running deployment commands.

We used environment variables such as `MYSQL_PASSWORD`, `MYSQL_DATABASE`, and `MYSQL_USER` to provide the configuration needed by Nextcloud and MariaDB. These variables allow the application to connect to the correct database using matching credentials and settings. I also learned that sample passwords should only be used in a laboratory environment and that real deployments require stronger security practices.

Deploying Nextcloud and MariaDB in just a few minutes felt exciting and rewarding. Seeing the Nextcloud installation page in my browser showed me that the containers were communicating and that the application was accessible. I also learned the importance of checking container status and properly shutting down the services after completing the activity.

Since Mission 1, my understanding of Cloud Computing has improved significantly. I now understand that cloud engineering involves more than simply running individual applications. It also requires managing multiple services, configuring networks, automating deployments, documenting infrastructure, and following security practices. This mission helped me appreciate how Docker Compose and Infrastructure as Code make cloud deployments more efficient, consistent, and manageable.
