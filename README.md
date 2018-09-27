# docker-centos6-i386-qt4.8 

This repository have a Dockerfile that extends the docker image [toopher/centos-i386:centos6](https://github.com/toopher/toopher-docker/tree/master/centos6-i386), this upgrade supports the qt4.8.

To build the docker image use:
```
docker build -t docker-centos6-i386-qt4.8:latest .
```
To run your application:
```
docker run --rm -ti -v $(pwd):/app docker-centos6-i386-qt4.8:latest /usr/lib/qt48/bin/qmake-qt4 && make
```
