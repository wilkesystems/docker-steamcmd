FROM opensuse:42.1

MAINTAINER wilkesystems <maintainer@wilke.systems>

ADD steamcmd.tar.xz /

RUN zypper install -y glibc-32bit libstdc++6-32bit net-tools; \
steamcmd +quit; rm -rf /root/.steam/logs/* /tmp/*

CMD ["steamcmd"]