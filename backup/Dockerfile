FROM php:7.3.7-cli-alpine3.10

RUN apk update && apk upgrade \
    && wget https://phar.phpbu.de/phpbu-6.0.0.phar \
    && chmod +x phpbu-6.0.0.phar \
    && mv phpbu-6.0.0.phar /usr/local/bin/phpbu

WORKDIR /data

CMD ["phpbu", "--configuration=backup-config.xml"]
