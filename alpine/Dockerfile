FROM openresty/openresty:alpine

RUN set -ex \
    && sed -i 's/dl-cdn.alpinelinux.org/mirrors.aliyun.com/g' /etc/apk/repositories \
    && apk add --no-cache ca-certificates tzdata \
    && rm -rf/var/cache/apk/* \
    && update-ca-certificates

ENV TZ=Asia/Shanghai