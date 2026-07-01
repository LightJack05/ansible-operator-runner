FROM alpine:latest

RUN apk add git bash ansible

RUN mkdir -p /playbook /deps/roles /deps/collections

COPY entrypoint.sh /entrypoint.sh

ENTRYPOINT ["/entrypoint.sh"]
