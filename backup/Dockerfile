FROM php:7.3.7-cli-alpine3.10

RUN apk update && apk upgrade \
    && wget https://phar.phpbu.de/phpbu-5.2.7.phar \
    && chmod +x phpbu-5.2.7.phar \
    && mv phpbu-5.2.7.phar /usr/local/bin/phpbu

WORKDIR /data

CMD ["phpbu", "--configuration=backup-config.xml"]
