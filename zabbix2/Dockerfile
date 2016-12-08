
FROM monitoringartist/zabbix-xxl:latest

EXPOSE 8083
EXPOSE 80

VOLUME ["/etc/localtime:/etc/localtime:ro"]

ENV ZS_DBHost=zabbix.db
ENV ZS_DBUser=zabbix
ENV ZS_DBPassword=admin

#-------------Run commands----------------#
#docker run -d -v /var/lib/mysql --name zabbixstorage busybox
#docker run -d --name zabbixdb --volumes-from zabbixstorage zabbixdb
#docker run -d --name zabbix -p 80:80 -p 8083:10051 --link zabbixdb:zabbix.db zabbix
