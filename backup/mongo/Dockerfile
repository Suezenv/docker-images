FROM suezenv/phpbu:5.2.7

RUN echo 'http://dl-cdn.alpinelinux.org/alpine/v3.9/community' >> /etc/apk/repositories
RUN apk update
RUN apk add mongodb-tools

WORKDIR /data
