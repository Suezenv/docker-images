FROM php:8.4.19-cli-alpine3.23

RUN apk update && apk upgrade \
    && wget https://phar.phpbu.de/phpbu-6.0.31.phar \
    && chmod +x phpbu-6.0.31.phar \
    && mv phpbu-6.0.31.phar /usr/local/bin/phpbu

WORKDIR /data

CMD ["phpbu", "--configuration=backup-config.xml"]
