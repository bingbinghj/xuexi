FROM centos:7

ENV TZ=Asia/Shanghai \
    LANG=C.UTF-8
    
WORKDIR /etc/sillyGirl

#VOLUME /etc/sillyGirl

ADD ["https://raw.githubusercontent.com/cdle/sillyGirl/main/install.sh","/usr/local/"]

RUN chmod +x /usr/local/install.sh

RUN cd && cd /usr/local/ && ./install.sh

RUN rm -rf /usr/local/install.sh

CMD ["/usr/local/sillyGirl/sillyGirl", "-t"]
