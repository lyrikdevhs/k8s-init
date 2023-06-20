FROM alpine:3.18

ENV NGINX_VERSION 1.16
ENV ALPINE_REPOSYTORY_URL 123

RUN apk add --no-cache --repository https://dl-cdn.alpinelinux.org/alpine/v3.18/main/ nginx=${NGINX_VERSION} \
 && mkdir -p /run/nginx

EXPOSE 80

COPY custom.conf /etc/nginx/conf.d/

COPY . /opt/

CMD ["nginx", "-g", "daemon off;"]

# size 9.25 MB
