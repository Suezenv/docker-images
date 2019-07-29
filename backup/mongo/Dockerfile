FROM suezenv/phpbu:5.2.7

RUN echo 'http://dl-cdn.alpinelinux.org/alpine/v3.9/community' >> /etc/apk/repositories \
    && apk update \
    && apk add mongodb-tools=4.0.5-r0

WORKDIR /data
