# dockerfile for image rawevan/ubuntu:shutter
# docker run -it --rm -v $(PWD):/home/developer/workspace rawevan/ubuntu:shutter
FROM rawevan/ubuntu:basetools
MAINTAINER Evan <liaiwen_mail@163.com>
RUN apt-get install -y shutter --no-install-recommends
ENV GOPATH /home/developer/workspace
ENV HOME /home/developer/workspace
CMD ["shutter"]

