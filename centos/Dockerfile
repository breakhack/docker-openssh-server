FROM centos

RUN yum install -y openssh-server vim
RUN ssh-keygen -A
COPY ./authorized_keys /root/.ssh/authorized_keys

ENTRYPOINT ["/usr/sbin/sshd", "-D"]