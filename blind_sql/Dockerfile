FROM php:7.3.3-apache-stretch

COPY src/ /var/www/html/

RUN set -ex \
    \
    && apt-get update \
    && apt-get install --assume-yes sqlite \
    \
    && chmod -R 777 /var/www/html/youwillnevereverfindthisdb.db \
    \
    && rm -rf /var/lib/apt/lists/*

EXPOSE 80
