FROM jenkinsci/blueocean

USER root

# install maven
RUN apk update && apk upgrade && apk add maven 

COPY plugins.txt /plugins.txt
RUN /usr/local/bin/plugins.sh /plugins.txt

