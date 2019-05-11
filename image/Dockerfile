FROM centos:centos7
RUN yum clean all && yum install -y epel-release && \
    yum install -y x11vnc \
    xorg-x11-server-Xvfb \
    xorg-x11-utils \
    which \
    qemu-kvm
COPY hdd.img /
COPY snapshot.img /
COPY entrypoint.sh /
ENTRYPOINT ["/entrypoint.sh"]
