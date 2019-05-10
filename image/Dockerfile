FROM centos:centos7
RUN yum clean all && yum install -y \
    xorg-x11-server-Xvfb \
    which \
    qemu-kvm
COPY hdd.img /
COPY snapshot.img /
COPY entrypoint.sh /
ENTRYPOINT ["/entrypoint.sh"]
