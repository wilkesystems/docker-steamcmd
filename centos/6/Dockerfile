FROM centos:6

MAINTAINER wilkesystems <maintainer@wilke.systems>

ADD steamcmd.tar.xz /

RUN yum update -y; yum -y install glibc.i686 libstdc++.i686 tbb.i686; \
steamcmd +quit; rm -rf /root/.steam/logs/* /tmp/*

CMD ["steamcmd"]