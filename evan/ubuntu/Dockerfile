# Dockerfile for rawevan/ubuntu:basetools
FROM rawevan/ubuntu:basetools
MAINTAINER Evan <liaiwen_mail@163.com>

RUN mv /sources.list /etc/apt/sources.list && \
    apt-get update && \
    apt-get upgrade -y 

ENV HOME /root
WORKDIR $HOME
