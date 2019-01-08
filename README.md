Simple Docker PHP Structure

Includes

- Nginx
- PHP
- Composer
- Mysql
- MongoDB

Usage

- Make sure you have docker and docker-compose installed in your machine.
- Edit the composer.json file with your configs and the packages required by your project.
- If you have some mysql data to import, set the files in the data/init_data folder and make sure you edit the name of the file on the Mysql section in the docker-compose.yml file. It will accepted .gz, .sql, etc...
- Run docker-compose up --build

URLs / Hostnames in the guest system

PHP - localhost:81
MySQL - localhost:82
