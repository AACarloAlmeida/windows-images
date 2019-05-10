FROM centos:centos7
RUN yum clean all && yum install -y \
    xvfb
    x11-utils \
    x11vnc    \
    qemu
COPY hdd.img /
COPY snapshot.img /
COPY entrypoint.sh /
ENTRYPOINT ["/entrypoint.sh"]
