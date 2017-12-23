FROM opensuse:42.2

MAINTAINER wilkesystems <maintainer@wilke.systems>

ADD steamcmd.tar.xz /

RUN zypper install -y glibc-32bit libstdc++6-32bit libtbb2 net-tools; \
steamcmd +quit; rm -rf /root/.steam/logs/* /tmp/*

CMD ["steamcmd"]