FROM php:7.0-fpm-alpine

MAINTAINER Jakub Cegiełka <kuba.ceg@gmail.com>

# RUN apk add --update \
#     php7-bcmath \
#     php7-mbstring


RUN rm -rf /var/cache/apk/* && rm -rf /tmp/*

CMD ["php-fpm", "-F"]

EXPOSE 9000