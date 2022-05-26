# Dockerfile for Wordpress

[Dockerfile](Dockerfile)

How to build:

```
docker build -t maiconpintopro/wordpress .
```

How to run:

```
docker run -d --rm --name mysql -v $PWD/data:/var/lib/mysql -e MYSQL_ROOT_PASSWORD=root maiconpintopro/mysql
docker exec -it mysql mysql -uroot -proot
mysql> create database wordpress;
docker run -d --rm --name wordpress -p 8000:80 maiconpintopro/wordpress
```

Database: wordpress
User: root
Password: root
Host: 172.17.0.2 // `docker inspect mysql` IpAddress
Prefix: wp_
