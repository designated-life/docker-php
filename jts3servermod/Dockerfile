FROM php:7.1-fpm-alpine
RUN apk update && apk add \
        # nproc
        coreutils \
        # php-mcrypt
        libmcrypt-dev \
    && docker-php-ext-install -j$(nproc) mcrypt mysqli
