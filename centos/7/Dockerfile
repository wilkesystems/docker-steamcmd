FROM centos:7

MAINTAINER wilkesystems <maintainer@wilke.systems>

ADD steamcmd.tar.xz /

RUN yum update -y; yum -y install glibc.i686 libstdc++.i686 net-tools; \
steamcmd +quit; rm -rf /root/.steam/logs/* /tmp/*

CMD ["steamcmd"]