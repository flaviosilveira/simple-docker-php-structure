# Simple Docker PHP Structure

## Containers
- Nginx
- PHP
- Composer
- Mysql
- MongoDB
- RabbitMQ

## How to use
- Make sure you have docker and docker-compose installed.
- Edit the composer.json file with your configs and the packages required by your project.
- If you have some mysql data to import, set the files in the data/init_data/mysql folder. Uncomment the line on Mysql section in the docker-compose.yml file and make sure you replaced the example for the name of your file. It will accepted .gz, .sql, etc... They will be executed in alphabetic order.
- If you have some mongoDB data to import, set the files in the data/init_data/mongo folder. Uncomment the line on Mongo section in the docker-compose.yml file and make sure you replaced the example for the name of your file. It will accepted .js and .sh. They will be executed in alphabetic order.
- Run docker-compose up --build

### Important
- If you import some data to mongoDB, it will use the users and passwords set on it. Environment variables in docker-compose.yml file will be ignored.

## URLs / Address in the guest system
- PHP - localhost:81
- MySQL - localhost:82
- MongoDB - localhost:83
- RabbitMQ - localhost:84

## Users and Passwords
- MySQL - root - 1234
- MongoDB - root - 1234
- RabbitMQ - guest - guest
