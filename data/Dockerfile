FROM alpine:3

RUN set -xe \
    && apk add --no-cache nodejs npm \
    && npm install -g json-server \
    && rm -rf /tmp/npm* /var/cache/apk/*

WORKDIR /data

EXPOSE 3000

ENTRYPOINT ["json-server"]
CMD ["--help"]