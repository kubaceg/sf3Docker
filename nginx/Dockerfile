FROM alpine:3.4

MAINTAINER Jakub Cegiełka <kuba.ceg@gmail.com>

RUN apk add --update nginx
RUN rm -rf /var/cache/apk/* && rm -rf /tmp/*

ADD nginx.conf /etc/nginx/
ADD symfony.conf /etc/nginx/conf.d/

RUN echo "upstream php-upstream { server php:9000; }" > /etc/nginx/conf.d/upstream.conf

RUN adduser -D -g '' -G www-data www-data

CMD ["nginx"]

EXPOSE 80
EXPOSE 443