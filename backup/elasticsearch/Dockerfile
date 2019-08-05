FROM suezenv/phpbu:5.2.7

RUN apk add nodejs=10.16.0-r0 \
    && apk add nodejs-npm

RUN npm install elasticdump@6.3.3 -g

WORKDIR /data
