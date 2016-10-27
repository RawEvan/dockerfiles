# lxde docker image base
FROM rawevan/ubuntu:basetools
MAINTAINER Evan <liaiwen_mail@163.com>

# install wine
RUN apt-get update && apt-get install -y xorg lxde-core tightvncserver --no-install-recommends
ENV HOME /root
WORKDIR $HOME
