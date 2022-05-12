# Dockerfile for CakePHP

[Dockerfile](Dockerfile)

How to build:

```
docker build -t maiconpintopro/cakephp .
```

How to run:

```
docker run -d --rm --name cakephp -v $PWD:/var/www/html -p 8888:80 -u $(id -u):$(id -g) maiconpintopro/cakephp
```
