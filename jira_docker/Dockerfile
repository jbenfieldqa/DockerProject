FROM ubuntu

RUN apt-get update


COPY response.varfile /responce.varfile
ADD https://www.atlassian.com/software/jira/downloads/binary/atlassian-jira-software-7.2.3-x64.bin /atlassian-jira-software-7.2.3-x64.bin
RUN chmod a+x atlassian-jira-software-7.2.3-x64.bin
COPY response.varfile /response.varfile

RUN ./atlassian-jira-software-7.2.3-x64.bin -q -varfile response.varfile

ENTRYPOINT ./atlassian/jira/bin/start-jira.sh -fg


