

# Used Docker Images
- [MariaDB](https://hub.docker.com/_/mariadb)
- [Wordpress](https://hub.docker.com/_/wordpress)
- [FTP](https://hub.docker.com/r/stilliard/pure-ftpd/)
- [Traefik (reverse proxy)](https://hub.docker.com/_/traefik)

# Setup server and install and setup Traefik
Before use, first setup your server and install and setup Traefik. Use this [tutorial](https://www.digitalocean.com/community/tutorials/how-to-use-traefik-as-a-reverse-proxy-for-docker-containers-on-ubuntu-18-04)(Only the server setup and Traefik part)

# Env
copy the example file to .env and change the values

    $ cp .env.example .env
    
# Run
start server

    $ docker-compose up -d

start server en verwijder alle containers die niet meer gebruikt worden

    $ docker-compose up -d --remove-orphans

stop server
    
    $ docker-compose down

stop server and remove files/database

    $ docker-compose down --volumes


