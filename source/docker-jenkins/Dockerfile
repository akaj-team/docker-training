FROM jenkinsci/blueocean

USER root

RUN apk update \
    && apk upgrade

COPY plugins.txt /plugins.txt
RUN /usr/local/bin/plugins.sh /plugins.txt

