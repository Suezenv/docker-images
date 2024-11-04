FROM php:8.3.12-cli-alpine3.20

RUN apk update && apk upgrade \
    && wget https://phar.phpbu.de/phpbu-6.0.23.phar \
    && chmod +x phpbu-6.0.23.phar \
    && mv phpbu-6.0.23.phar /usr/local/bin/phpbu

WORKDIR /data

CMD ["phpbu", "--configuration=backup-config.xml"]
