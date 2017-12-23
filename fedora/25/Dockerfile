FROM fedora:25

MAINTAINER wilkesystems <maintainer@wilke.systems>

ADD steamcmd.tar.xz /

RUN dnf install -y binutils glibc.i686 libstdc++.i686 tbb.i686 net-tools; \
steamcmd +quit; rm -rf /root/.steam/logs/* /var/lib/dnf/* /tmp/*

CMD ["steamcmd"]