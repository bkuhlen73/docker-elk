#ARG  ELK_VERSION
#FROM bkuhlen73/ubuntu:${ELK_VERSION}
#
#ENV TERM=xterm
## Add your elasticsearch plugins setup here
## Example: RUN elasticsearch-plugin install analysis-icu
#
#RUN ["/usr/bin/metricbeat", "-e"]
FROM ubuntu:latest

RUN apt-get -y update
RUN apt-get -y upgrade
RUN apt-get install -y joe
RUN apt-get install -y curl
RUN curl -L -O https://artifacts.elastic.co/downloads/beats/filebeat/filebeat-6.6.0-amd64.deb
RUN dpkg -i filebeat-6.6.0-amd64.deb
CMD ["/usr/bin/filebeat", "-e"]
