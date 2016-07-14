# Docker based development env for PHP

This is a docker based development env. Highly opinionated to suit my personal needs.

The env currently runs the following stack :

- Nginx
- php-fpm with PHP 5.5
- mysql 5.6

You can tweak the Dockerfiles for your own needs.

- PHP - php-fpm/Dockerfile
- mysql - mysql/Dockerfile

Also mysql/data folder is used to persist the database. The volume is mounted
to /var/lib/mysql within the container.

MySQL has a default account :

- Username : root
- Password : root

The server is publicly accessible. ( mysql/entrypoint.sh )
