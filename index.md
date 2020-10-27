# Laravel + Docker = :heart: :computer:

## Required

> You need to have installed next software.

-   Docker
-   PHP
-   Composer

## Installation

```bash
$ git clone https://github.com/luchoweb/Laravel-Docker.git
$ cd Laravel-Docker
$ composer install
$ docker-compose up -d
```

## Create MySQL user

```bash
$ docker exec -it laravel_db ./bin/bash
$ mysql -u root -p (password: 14r4ve1)
$ mysql> GRANT ALL ON laravel.* TO 'laraveluser'@'localhost' IDENTIFIED BY '14r4ve1';
$ mysql> FLUSH PRIVILEGES;
$ mysql> EXIT;
$ exit
```

> You can test with **bash** instead of **./bin/bash** if use Linux or Mac.

Ready!
Now you can go to http://localhost:8080
> You can change this port (8080) in docker-compose.yml 

Happy coding!
