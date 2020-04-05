

# Used Docker Images
- [MariaDB](https://hub.docker.com/_/mariadb)
- [Wordpress](https://hub.docker.com/_/wordpress)
- [FTP](https://hub.docker.com/r/stilliard/pure-ftpd/)
- [Traefik](https://hub.docker.com/_/traefik)


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


