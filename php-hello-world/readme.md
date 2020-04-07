# Simple Web Application

This is a simple web application using [php:7.2-apache image](https://github.com/docker-library/php/blob/03574f961844ad2a56d4c2c5304ffb30d3bfdc2b/7.2/buster/apache/Dockerfile).  

## 1. Use php image
  
    FROM php:7.2-apache
   
## 2. Copy our index file

    COPY index.php /var/www/html

## 3. Start the container with a pre-built image

    docker run -p 8080:80 dwhitz/php-hello-world

## 4. Get the IP of your container

Get your container id
    
    docker ps -q

Retrieve the IP Address 

    docker inspect <container-id>

## 5. Test

Open a browser and go to URL

    http://<IP>:8080  =>  Hello World from index.php!
