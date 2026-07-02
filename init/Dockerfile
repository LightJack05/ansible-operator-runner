FROM alpine:latest

RUN apk add bash ansible openssh-client \
  python3 py3-pip \
  sshpass sudo \
  bash coreutils findutils grep sed tar gzip xz shadow util-linux \
  git rsync unzip ca-certificates openssl iproute2 procps

RUN mkdir -p /playbook /deps/roles /deps/collections

COPY entrypoint.sh /entrypoint.sh

ENTRYPOINT ["/entrypoint.sh"]
