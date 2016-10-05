FROM alpine:edge
MAINTAINER Philip Graf <mail@philipgraf.de>

ADD rootfs /

RUN apk update && \
  apk upgrade && \
  apk add \
    ca-certificates \
    curl \
    bash \
    tar \
    s6 \
    confd@testing && \
  rm -rf /var/cache/apk/*

ENV TERM xterm
CMD ["bash"]
