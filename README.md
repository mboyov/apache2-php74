# Docker stack web by mboyov

- DockerHub : [mboyov/apache2-php74](https://hub.docker.com/r/mboyov/apache2-php74/)
 
## PHP applications on Apache

- Ubuntu 18.04

- Apache 2

- PHP 7.4

## Build

To create the base image mboyov/apache2-php74, execute the following command:

`docker build -t mboyov/apache2-php74 .`

Running your Apache and PHP docker image

Start your image binding the external ports 80 in all interfaces to your container:

`docker run -d -p 80:80 mboyov/apache2-php74`

## Compose

In the docker-compose.yml file replace the volume line "/var/www" with your working directory and execute the following command:

`docker-compose up`