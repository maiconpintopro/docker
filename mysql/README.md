# Dockerfile for Mysql

[Dockerfile](Dockerfile)

How to build:

```
docker build -t maiconpintopro/mysql .
```

How to run:

```
docker run -d --name mysql -v $PWD/data:/var/lib/mysql -e MYSQL_ROOT_PASSWORD=root -e MYSQL_DATABASE=mydbname maiconpintopro/mysql
```
