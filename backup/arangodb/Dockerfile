
ARG PHPBU_VERSION=6.0.5
FROM suezenv/phpbu:${PHPBU_VERSION}

RUN apk --no-cache add ca-certificates
ADD ZscalerRootCertificate-2048-SHA256.crt /usr/local/share/ca-certificates/ZscalerRootCertificate-2048-SHA256.crt
RUN chmod 644 /usr/local/share/ca-certificates/ZscalerRootCertificate-2048-SHA256.crt \
    && update-ca-certificates

ARG ARANGODB_VERSION=3.10.5
RUN echo "Install ArangDB Client tools version : ${ARANGODB_VERSION}" \
    && wget --timeout=600 https://download.arangodb.com/arangodb310/Community/Linux/arangodb3-client-linux-${ARANGODB_VERSION}_x86_64.tar.gz \
    && tar xvf arangodb3-client-linux-${ARANGODB_VERSION}_x86_64.tar.gz --strip-components=1 -C / \
    && rm arangodb3-client-linux-${ARANGODB_VERSION}_x86_64.tar.gz \
    && mkdir -p /etc/arangodb3 \
    && touch /etc/arangodb3/arangodump.conf \
    && echo 'overwrite=true' >> /etc/arangodb3/arangodump.conf \
    && echo 'all-databases=true' >> /etc/arangodb3/arangodump.conf

WORKDIR /data
