# jenkins-docker-run-inside

[![](https://img.shields.io/docker/stars/jesusperales/jenkins-docker-run-inside.svg)](https://hub.docker.com/r/jesusperales/jenkins-docker-run-inside/ 'Docker hub')
[![](https://img.shields.io/docker/pulls/jesusperales/jenkins-docker-run-inside.svg)](https://hub.docker.com/r/jesusperales/jenkins-docker-run-inside/ 'Docker hub')

This image permits run docker commands inside of jenkins container.

## Instructions

* `docker pull jesusperales/jenkins-docker-run-inside`

* `docker run --name jenkins -d -p 8080:8080 -p 50000:50000 -v /var/run/docker.sock:/var/run/docker.sock -v $(which docker):$(which docker) jesusperales/jenkins-docker-run-inside`

* `docker exec -it jenkins /bin/bash`

* `docker ps -a`

## Tested on

* Ubuntu 16.04

## See about

 * [stackoverflow](https://stackoverflow.com/questions/45121945/jenkins-in-docker-container-run-docker-pipeline)

* [Jenkins official image](https://hub.docker.com/r/jenkins/jenkins/)
