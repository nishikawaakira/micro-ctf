FROM php:8.0-fpm

RUN apt-get update && apt-get upgrade -y \
  && docker-php-ext-install pdo_mysql mysqli \
  && apt-get clean \
  && rm -rf /var/lib/apt/lists/*

WORKDIR /var/www/html

EXPOSE 80