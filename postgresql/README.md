# Dockerfile for PostgreSQL

[Dockerfile](Dockerfile)

How to build:

```
docker build -t maiconpintopro/postgresql .
```

How to run:

```
docker run -d --rm --name postgresql -v $PWD/data:/var/lib/postgresql/data -e POSTGRES_PASSWORD=root maiconpintopro/postgresql
```
