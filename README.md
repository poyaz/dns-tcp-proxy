Introduction
============

Sample HTTP/HTTPS proxy in TCP layer and use for dns proxy


Requirement
===========

This project run very sample and easy. Just need `docker` and `docker-compose` and then start

Environment
===========

For set proxy ip Address you have to use `PROXY_IP_ADDRESS` environment.

* Example:

```bash
PROXY_IP_ADDRESS=192.168.20.30
```

Usage
=====

How to use in production?

```bash
# run in port 80, 443

PROXY_IP_ADDRESS=<your-public-ip-address> docker-compose up -d
```

Use in test with sample http server

```bash
PROXY_IP_ADDRESS=<your-public-ip-address> docker-compose -f docker-compose.yml -f docker/docker-compose.sample.yml up -d

curl http://ifconfig.io
curl https://ifconfig.io
```
