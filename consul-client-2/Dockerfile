FROM debian:latest

RUN apt-get update && apt-get upgrade && apt-get -y install unzip 

ADD https://releases.hashicorp.com/consul/0.7.5/consul_0.7.5_linux_amd64.zip /tmp/consul.zip

RUN cd /usr/local/bin && unzip /tmp/consul.zip && chmod +x /usr/local/bin/consul

ADD https://releases.hashicorp.com/consul/0.7.5/consul_0.7.5_web_ui.zip /tmp/webui.zip

RUN cd /opt && unzip /tmp/webui.zip

EXPOSE 8300 8301 8301/udp 8302 8302/udp 8400 8500 53/udp 

VOLUME ["/consul/data"]

ENV SHELL /bin/bash ENTRYPOINT ["/bin/start"]

CMD []

