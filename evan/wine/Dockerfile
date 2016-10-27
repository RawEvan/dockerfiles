# Wine docker image base
FROM rawevan/ubuntu:basetools
MAINTAINER Evan <liaiwen_mail@163.com>

# install wine
RUN apt-get update && apt-get install -y python-software-properties --no-install-recommends && \
    add-apt-repository ppa:ubuntu-wine/ppa && \
    apt-get update && \
    apt-get install -y wine --no-install-recommends && \
	dpkg --add-architecture i386 && \
	apt-get update && \
	apt-get install -y \
	wine32 \
	--no-install-recommends \
	&& rm -rf /var/lib/apt/lists/*

ENV HOME /root
WORKDIR $HOME
