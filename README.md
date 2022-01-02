Introduction
============

Sample HTTP/HTTPS proxy in TCP layer and use for dns proxy


Requirement
===========

This project run very sample and easy. Just need `docker` and `docker-compose` and then start


Usage
=====

How to use in production?

```bash
# run in port 80, 443

docker-compose up -d
```

Use in test with sample http server

```bash
docker-compose -f docker-compose.yml -f docker/docker-compose.sample.yml up -d

curl http://localhost:80
```
