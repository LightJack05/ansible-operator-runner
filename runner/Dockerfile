FROM alpine:latest

RUN apk add bash ansible openssh-client \
  python3 py3-pip \
  sshpass sudo \
  bash coreutils findutils grep sed tar gzip xz shadow util-linux \
  git rsync unzip ca-certificates openssl iproute2 procps

RUN mkdir -p /etc/ansible

COPY ansible.cfg /etc/ansible/ansible.cfg
COPY entrypoint.sh /entrypoint.sh

ENTRYPOINT ["/entrypoint.sh"]
