FROM jenkinsci/blueocean

USER root

RUN apk update \
    && apk upgrade
# install maven
RUN apk update && apk upgrade && apk add maven 

COPY plugins.txt /plugins.txt
RUN /usr/local/bin/plugins.sh /plugins.txt

