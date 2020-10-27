# Laravel/Docker

## Required

-   Docker
-   PHP
-   Composer

> You need to have previously installed the previous software.

## Installation

-   Clone repo
-   Run "cd laravel-docker"
-   Run "composer install"
-   Run "docker-compose up -d"

## Create MySQL user

-   Run "docker exec -it laravel_db ./bin/bash" (Using Git Bash from Windows)
-   mysql -u root -p (password: 14r4ve1)
    > You can change this password in docker-compose.yml, mysql/.env & .env
-   Run "GRANT ALL ON laravel.\* TO 'laraveluser'@'localhost' IDENTIFIED BY '14r4ve1';"
-   Run "FLUSH PRIVILEGES;"
-   Run "EXIT;"
-   Run "exit"

Ready!
Now you can go to http://localhost:8080
> You can change this port (8080) in docker-compose.yml 

Happy coding!
