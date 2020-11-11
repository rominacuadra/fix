# Larvel + Apache + Mysql + Docker
Laravel skeleton for new proyect

## Webserver image for Laravel
`php:7.3-apache` 

## Database image 
`mysql:8.0`

## Up and running

1. Clone the repo:
```
    $ git clone https://github.com/rominacuadra/larvel.git
```    

2. Rename the folder for your new proyect then enter folder:
```    
    $ cd [NEWNAME]
```    

3. Copy .env.example to .env:
```
    $ cp .env.example .env 
```    
    
4. Build the images and start the services:
```
    $ docker-compose build
    $ docker-compose up -d
```

5. Check created containers:
```
    $ docker ps
```

6. Install compose and configure artisan in app container:
```
    $ docker exec -it laravel-app bash
    $ composer install
    $ php artisan key:generate
    $ php artisan migrate
```

7. Add new host in hostfile: /etc/hosts
```
    127.0.0.1       laravel-app.local
```

8. Check URL:
` http://laravel-app.local:8000`

9. Go to
