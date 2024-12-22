FROM bitrixdock/php56-fpm:latest

ARG SITE_PATH

LABEL org.opencontainers.image.source="https://github.com/frizus/bitrixdock"

COPY ./php.ini /etc/php5/fpm/conf.d/90-php.ini
COPY ./php.ini /etc/php5/cli/conf.d/90-php.ini

RUN usermod -u 1000 www-data

WORKDIR ${SITE_PATH}

EXPOSE 9000
