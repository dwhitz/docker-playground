# Docker compose for a custom Web Application

## 1. Start all services

    docker-compose up

## 2. Check the mapped port

    docker ps 

 The port will be mapped as follows
>     0.0.0.0:8090->8080/tcp

## 3. Get the IP of your webapp

    docker ps -q

 Retrieve the IP Address

    docker inspect <container-id>

## 4. Test

 Open your browser and go to

    http://<IP>:8090            => Welcome
    http://<IP>:8090\hello      => Hello World!
