FROM ubuntu

RUN  apt-get update -y
RUN  apt-get install -y  default-jre default-jdk

ADD http://download.sonatype.com/nexus/3/latest-unix.tar.gz latest-unix.tar.gz
RUN tar zxvf latest-unix.tar.gz
RUN chmod a+x /nexus-3.1.0-04/bin/nexus
WORKDIR /nexus-3.1.0-04/bin

EXPOSE 808

ENTRYPOINT ./nexus  start && bash


#----------------RUN COMMAND---------------#
#docker run -p 8085:8081 -dti nexustest bash 


