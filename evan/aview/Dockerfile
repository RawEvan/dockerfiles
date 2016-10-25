# dockerfile for image rawevan/ubuntu:aview
# docker run -it --rm -v $(PWD):/home/developer/workspace rawevan/ubuntu:aview
FROM rawevan/ubuntu:basetools
MAINTAINER Evan <liaiwen_mail@163.com>
RUN apt-get install -y aview --no-install-recommends && \
    apt-get install -y imagemagick --no-install-recommends && \
    rm -rf /var/lib/apt/lists/*
ENV GOPATH /home/developer/workspace
ENV HOME /home/developer/workspace
CMD ["asciiview"]

