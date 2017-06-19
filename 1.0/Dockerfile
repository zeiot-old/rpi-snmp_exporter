# VERSION 0.4.0
# AUTHOR:         Nicolas Lamirault <nicolas.lamirault@gmail.com>
# DESCRIPTION:    zeiot/rpi-snmp_exporter

FROM resin/armv7hf-debian:stretch
MAINTAINER Nicolas Lamirault <nicolas.lamirault@gmail.com>

ENV SNMP_EXPORTER_VERSION 0.4.0

ADD https://github.com/prometheus/snmp_exporter/releases/download/v${SNMP_EXPORTER_VERSION}/snmp_exporter-${SNMP_EXPORTER_VERSION}.linux-armv7.tar.gz /snmp_exporter.tar.gz

RUN tar -xf /snmp_exporter.tar.gz && \
    rm /snmp_exporter.tar.gz && \
    mv snmp_exporter-${SNMP_EXPORTER_VERSION}.linux-armv7/snmp_exporter /usr/bin/snmp_exporter && \ 
    rm -fr snmp_exporter-${SNMP_EXPORTER_VERSION}.linux-armv7

EXPOSE     9116

ENTRYPOINT [ "/usr/bin/snmp_exporter" ]
