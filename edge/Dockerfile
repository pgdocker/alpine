FROM alpine:edge
MAINTAINER Philip Graf <mail@philipgraf.de>

ADD rootfs /

RUN apk upgrade --no-cache && \
  apk add --no-cache \
    ca-certificates \
    curl \
    bash \
    tar \
    s6 \
    confd@testing

ENV TERM xterm
CMD ["bash"]
