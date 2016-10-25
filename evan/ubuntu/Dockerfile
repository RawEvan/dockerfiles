# Dockerfile for rawevan/ubuntu:basetools
FROM ubuntu:16.04
MAINTAINER Evan <liaiwen_mail@163.com>

ADD sources.list /etc/apt/sources.list
RUN apt-get update && \
    apt-get upgrade -y && \
    apt-get install -y wget && \
	rm -rf /var/lib/apt/lists/*

ENV HOME /root
WORKDIR $HOME
