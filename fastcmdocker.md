docker-compose up -d nginx mysql

docker exec -it test\_php-fpm\_1 /bin/bash

docker exec -it test\_lighttpd\_1 /bin/bash

crete database utf-8 CREATE DATABASE test\database CHARACTER SET
utf8 COLLATE utf8\_general\_ci;

docker exec -it test\_mysql\_1 /bin/bash docker restart c554c459c595

docker exec -i dockertest\_mysql\_1 mysql -uroot -psecret

test\database \< test\database.sql CREATE DATABASE

test\database CHARACTER SET utf8 COLLATE utf8\_general\_ci;

connect to container docker exec -it e4e46efdc4bb /bin/bash

close all containers docker stop \$(docker ps -a -q)

remove all container docker rm \$(docker ps -a -q)

remove all images docker rmi \$(docker images -q)

list containers docker ps -a

remove single container docker rm dockertest\_nginx\_1

IMPORTANT docker network inspect test\_default

sudo locale-gen se\_SE sudo locale-gen no\_NO

IMPORTANTE PER IL DATABASE:

    mysql:
        build: ./mysql
        ports:
           - "3306:3306"
        volumes_from:
            - volumes_data
        environment:
            MYSQL_DATABASE: test_platform
            MYSQL_USER: homestead
            MYSQL_PASSWORD: secret
            MYSQL_ROOT_PASSWORD: root 


IMPORTANT CHECK NETWORK PORTS

sudo lsof -i -P | grep -i "listen"


CREATE DATABASE CREATE DATABASE test\database CHARACTER SET utf8
COLLATE utf8\_general\_ci;

WHIRESHARK filter: ip.addr == 127.0.0.1

COMMANDS CONNECT TO CONTAINER OR TO ENTER SHELL ALPINE
RUN /bin/ash FOR Alpine
Options used above:
/bin/ash is Ash (Almquist Shell) provided by BusyBox
--rm Automatically remove the container when it exits (docker run --help)
Use this:
docker exec -it test\_php-fpm\_1   /bin/ash

Info :https://en.wikipedia.org/wiki/Almquist\_shell


AFTER INTSTAL nano
Run comand : export TERM=xterm

LINK IMPORTANT
https://github.com/matriphe/docker-alpine-php
https://github.com/matriphe/docker-alpine-nginx/issues/1
