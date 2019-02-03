# docker-everythings

## Databases

1. Mysql

    docker run --name mysql -v /data/mysql:/var/lib/mysql -v /data/sql:/sql -e MYSQL_ROOT_PASSWORD=rootpass -p 3306:3306 --restart always -d mysql:5.7

## Message Queue

1. RabbitMQ

    docker run -d --name rabbit --hostname rabbit -v /data/rabbit:/var/lib/rabbitmq -p 5672:5672 --restart always rabbitmq:3