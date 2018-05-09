# Simple work with RabbitMQ via PHP

![](https://avatars0.githubusercontent.com/u/96669?s=200&v=4)



## Installation

You can install RabbitMQ via docker.

1. Install docker
[Ubuntu](https://docs.docker.com/install/linux/ubuntu/)
[Mac](https://docs.docker.com/docker-for-mac/install/)
[Windows](https://docs.docker.com/docker-for-windows/install/)

2. Pull docker image.
 ```
 docker pull rabbitmq
 ```

3.  Run container with RabbitMQ.
```
sudo docker run -d --hostname my-rabbit --name rabbit-web -p 8080:15672 -p 5672:5672 rabbitmq:3-management
```

4. Open RabbitMQ management web.
```
http://127.0.0.1:8080
username: guest
pwd: guest
```

5. Clone project. 
```
git clone git@github.com:Rishats/php-amqplib-learn.git rabbit.test
```

6. Install dependency. 
```
cd rabbit.test
composer install
```

7. Configure src files. 
```
If you run your server on your local machine you should use 127.0.0.1 ^)
I use 192.168.8.99 because i have my own home server ^). 
```

**How run scripts?**

Simple, just run scripts via php.

Example:
```
php send.php
php recieve.php
```




