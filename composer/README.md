# Dockerfile for Composer

[Dockerfile](Dockerfile)

How to build:

```
docker build -t maiconpintopro/composer .
```

How to run:

```
docker run --rm -v $PWD:/app -u $(id -u):$(id -g) maiconpintopro/composer
```

More examples:

```
docker run --rm -v $PWD:/app -u $(id -u):$(id -g) maiconpintopro/composer project1
docker run --rm --entrypoint composer maiconpintopro/composer --version
```
