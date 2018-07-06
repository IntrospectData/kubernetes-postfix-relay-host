FROM alpine:3.6
MAINTAINER Patrick McClory <pmdev@introspectdata.com>

RUN apk add --no-cache postfix rsyslog supervisor \
    && /usr/bin/newaliases

COPY . /

EXPOSE 25

ENTRYPOINT [ "/tx-smtp-relay.sh" ]
