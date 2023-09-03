# nginx-http-fileserver-docker

This repository contains a Docker Compose and Nginx configuration setup designed for serving files over HTTP. The service is configured to run on port 80 of your local machine and serve files located in the /data directory on your host system.
Components

docker-compose.yml: This is the Docker Compose file that orchestrates the container setup. It uses the latest Nginx image and maps port 8080 on the host to port 80 on the container. It also sets up a volume to serve files from your host's /data directory.

nginx.conf: The Nginx configuration file specifies the basic settings for the web server, such as listening on port 80 and enabling directory listing (autoindex on).

Quick Start

    Make sure you have Docker and Docker Compose installed on your machine.
    Clone this repository.
    Navigate to the directory containing docker-compose.yml.
    Run docker-compose up to start the Nginx file server.
    Open a web browser and navigate to http://localhost:8080 to access the files.

For more advanced configurations and settings, please refer to the nginx.conf file in the repository.
