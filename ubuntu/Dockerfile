FROM ubuntu

RUN apt update && \
    apt install -y openssh-server vim htop curl && \
    mkdir -p /run/sshd
#RUN echo 'PubkeyAuthentication yes' >> /etc/ssh/sshd_config
COPY ./authorized_keys /root/.ssh/authorized_keys

ENTRYPOINT ["/usr/sbin/sshd", "-D"]