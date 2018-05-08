FROM elicocorp/odoo-china:10.0
# reference: https://hub.docker.com/r/kongkoro/pycharm/~/dockerfile
# remove libs that already been listed in https://github.com/Elico-Corp/odoo-docker/blob/11.0/sources/apt.txt
RUN apt-get update &&\
    apt-get install -y \ 
        wget \ 
        libxtst6 \ 
        libxi6 \
        python-software-properties \
        software-properties-common \
        --no-install-recommends
RUN wget https://download.jetbrains.8686c.com/python/pycharm-community-2018.1.2.tar.gz -O /tmp/pycharm.tar.gz
RUN apt-get install -f && add-apt-repository ppa:openjdk-r/ppa && apt-get update && apt-get install openjdk-7-jre
RUN rm -rf /var/lib/apt-lists; rm -rf /tmp/*; apt-get purge wget -y; apt-get autoremove -y
ENV PYCHARM_HOME=/etc/pycharm
RUN mkdir ${PYCHARM_HOME} && tar -xzvf /tmp/pycharm.tar.gz -C ${PYCHARM_HOME} --strip=1
#ENTRYPOINT ["/etc/pycharm/bin/pycharm.sh"]
