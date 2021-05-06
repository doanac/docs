FROM alpine:latest

RUN apk add --no-cache --virtual .build-deps build-base py3-pip && \
    apk add --no-cache python3 python3-dev && \
    pip3 install --no-cache-dir mkdocs==1.1.2 mkdocs-macros-plugin==0.5.5 && \
    apk del .build-deps

