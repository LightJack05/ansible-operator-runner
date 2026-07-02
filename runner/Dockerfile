FROM alpine:latest

RUN apk add bash ansible

RUN mkdir -p /etc/ansible

COPY ansible.cfg /etc/ansible/ansible.cfg
COPY entrypoint.sh /entrypoint.sh

ENTRYPOINT ["/entrypoint.sh"]
