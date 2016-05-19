# Technocrat Signal

To use, install the [Docker Toolbox](https://www.docker.com/products/docker-toolbox) and [VirtualBox](https://www.virtualbox.org/wiki/Downloads).

Make sure you are using at least these versions:

```
$  docker-compose --version
docker-compose version 1.7.0, build 0d7bf73
$ docker-machine --version
docker-machine version 0.7.0, build a650a40
$ docker --version
Docker version 1.11.1, build 5604cbe
```

Then, run this command to build the playground (in a machine called "technocrat").

```
$ docker-machine create --driver virtualbox technocrat
$ docker-machine start technocrat
$ git clone https://github.com/xrd/technocrat-signal.git
$ cd technocrat-signal
$ eval $(docker-machine env technocrat)
$ docker-compose build  # go get a coffee
```