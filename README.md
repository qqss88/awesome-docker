Awesome Docker
==============

A community driven list of useful Docker links


## Docker online

*Try Docker online*

* [Docker](https://www.docker.com/tryit/) — Try Docker online

## Docker Management UI

* [dockerui](https://github.com/crosbymichael/dockerui)
* [Kitematic](https://kitematic.com/)
* [Shipyard](http://shipyard-project.com/)


## Use cases

* [Use cases](https://www.docker.com/resources/usecases/) 


## Docker hub

*Docker repositories*

* [Docker hub](https://registry.hub.docker.com/)


## Interesting and Useful Docker containers

*A list of useful Docker containers* 

* [Docker Image for Graphite](https://github.com/hopsoft/docker-graphite-statsd) - Graphite & Statsd can be a pain in the ass to setup. This Docker image will help you get up & running quickly.
* [phusion/baseimage-docker](http://phusion.github.io/baseimage-docker/) - A docker ubuntu 14.04 baseimage done right.
* [ZNC with Docker](https://github.com/shykes/docker-znc) - Run the ZNC irc bouncer on Docker 

## Useful Docker Articles(Chinese Version)

* [DockerOne - Docker中文交流平台](http://dockerone.com/) by [@李颖杰](http://dockerone.com/people/%E6%9D%8E%E9%A2%96%E6%9D%B0)

## Slides

*Great slides about Docker*

* [Ship with Docker](https://speakerdeck.com/slok/ship-it-with-docker)

## Commands

Share folder in container

via shell:
```shell
    $ docker run -v /path/to/code:/src \
    -i -t image /bin/bash
```
via dockerfile:

    FROM busybox
    VOLUME ["/var/volume1", "/var/volume2"]
    CMD ["/bin/true"]
    
Linked Containes
`use --link postgresql:pg`

    docker build -t postgresql .
    docker run -rm -p --name pg postgresql
    docker run -rm -t -i --link pg:pg postgresql bash
    psql -h pg -d docker -U docker --password

Port forwarding intro a container

in boot2docker:

    ssh -L 8000:localhost:8000
    
    

## Contributing

Your contributions are always welcome! Please submit a pull request or create an issue to add to the list. :thumbsup:


## License

[![Creative Commons License](http://i.creativecommons.org/l/by/4.0/88x31.png)](http://creativecommons.org/licenses/by/4.0/)

This work is licensed under a [Creative Commons Attribution 4.0 International License](http://creativecommons.org/licenses/by/4.0/).

