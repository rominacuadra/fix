# Larvel + Apache + Mysql + Docker
Laravel skeleton for new proyect

## Webserver image for Laravel
```
   php:7.3-apache
```   

## Up and running

1. Clone the repo:
    $ git clone https://github.com/rominacuadra/larvel.git

2. Rename the folder for your new proyect:
    $ cd [NEWNAME]

3. Copy .env.example to .env:
    $ cp .env.example .env 
    
4. Build the images and start the services:
    $ docker-compose build
    $ docker-compose up -d
