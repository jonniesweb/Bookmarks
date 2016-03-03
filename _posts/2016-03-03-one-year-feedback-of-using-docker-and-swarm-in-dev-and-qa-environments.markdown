---
layout: "post"
title: "One year+ feedback of using Docker and Swarm in DEV and QA environments"
date: "2016-03-03 13:13"
link: "https://medium.com/@frntn/one-year-feedback-of-using-docker-and-swarm-in-dev-and-qa-environments-deaf2ec6dc61#.p9k6clmjz"
summary: "An original use case showing Docker Swarm being used to scale and manage multiple environments"
tags:
 - docker
 - docker-swarm
---
The people over at Ekino have engineered their own workflow for having multiple environments using Docker Swarm. Presented in this article is the use case of two static pools of machines, within each are multiple environments that can be dynamically shifted. ie. The static QA pool of servers contains the integration, validation and performance testing environments. At the flick of a switch the operators are able to allocate more servers to the performance environment for better balancing of workload.

The authors are also practicing immutable infrastructure, with these environments. From within their Jenkins continuous integration server, they're able to wipe and freshly deploy an entire environment in three minutes.
