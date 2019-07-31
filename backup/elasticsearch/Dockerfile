FROM suezenv/phpbu:5.2.7

RUN apk add nodejs \
    && apk add nodejs-npm

RUN npm install elasticdump -g

WORKDIR /data
