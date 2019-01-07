# jslave

[![Build Status](https://travis-ci.org/hberndt/jslave.svg?branch=master)](https://travis-ci.org/hberndt/jslave)


Different Docker images for jenkins slaves

```
docker run -i --rm --name agent1 --init -v agent1-workdir:/home/jenkins/agent hberndt/jslave-jdk8 java -jar /usr/share/jenkins/slave.jar -workDir /home/jenkins/agent
```

To run with docker tooling

```
docker run -i --rm --name agent1 --init -v /var/run/docker.sock:/var/run/docker.sock -v agent1-workdir:/home/jenkins/agent hberndt/jslave-docker java -jar /usr/share/jenkins/slave.jar -workDir /home/jenkins/agent
```

## Images hosted on Docker Hub

- **hberndt/jslave8** [![Automated build](https://img.shields.io/docker/automated/hberndt/jslave.svg)](https://hub.docker.com/r/hberndt/jslave/) [![Docker Pulls](https://img.shields.io/docker/pulls/hberndt/jslave.svg)](https://hub.docker.com/v2/repositories/hberndt/jslave/)
