#ARG  ELK_VERSION
#FROM bkuhlen73/ubuntu:${ELK_VERSION}
#

## Add your elasticsearch plugins setup here
## Example: RUN elasticsearch-plugin install analysis-icu
#

FROM bkuhlen73/apachebeat:latest
ENV TERM=xterm
#RUN apt-get -y update
#RUN apt-get -y upgrade
#RUN apt-get install -y joe
#RUN apt-get install -y curl
#RUN curl -L -O https://artifacts.elastic.co/downloads/beats/filebeat/filebeat-6.6.0-amd64.deb
#RUN dpkg -i filebeat-6.6.0-amd64.deb
#CMD ["/usr/sbin/apachectl", "start"]
CMD ["/usr/bin/filebeat", "-e"]
#RUN ["source", "/etc/apache2/envvars"]
#EXPOSE 80
#CMD service apache2 start
##ENTRYPOINT ["/usr/sbin/apache2", "-k", "start"]
#EXPOSE 80

CMD ["/usr/sbin/apache2ctl", "-D", "FOREGROUND"]

