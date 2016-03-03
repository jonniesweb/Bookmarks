---
layout: "post"
title: "Using Docker-in-Docker for your CI or testing environment? Think twice"
date: "2016-03-03 12:13"
link: "http://jpetazzo.github.io/2015/09/03/do-not-use-docker-in-docker-for-ci/"
summary: "Don't run Docker-in-Docker, mount the socket instead!"
tags:
 - docker
---

It's becoming more common to utilize Docker to build and test software in containers, the main benefits being speed and lower resource utilization compared to virtual machines. Initially you may think that running Docker-in-Docker is the correct solution, but a much easier and lighter weight method is to pass the /var/run/docker.sock file into the container. This article comes from an early developer of Docker, so you know they're reputable.
