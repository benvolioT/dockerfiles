Nickstenning's Dockerfiles changed to work-around a Docker bug that prevents running on the Rackspace Cloud
===========

This repository contains a bunch of
[Dockerfiles](http://docs.docker.io/en/latest/use/builder/), which are
specifications of container images for [Docker](http://www.docker.io/).

For the most part, all these container images are published under my nickstenning's on
the Docker registry, at:

> <https://index.docker.io/u/nickstenning/>

However, due to a bug in Docker [#1984](https://github.com/dotcloud/docker/issues/1984) that is really caused by a bug in glibc LP: [eglibc/+bug/956051](https://bugs.launchpad.net/ubuntu/+source/eglibc/+bug/956051), these docker images fail to run properly on the Rackspace Cloud.  Therefore, I've created this fork to update the Dockerfiles to [work around the bug](https://journal.paul.querna.org/articles/2013/10/15/docker-ubuntu-on-rackspace/) until it is fixed.

