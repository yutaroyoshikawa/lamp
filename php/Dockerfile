FROM php:7-fpm
RUN apt-get update && apt-get install -y \
  libfreetype6-dev libjpeg62-turbo-dev libmcrypt-dev \
  git vim unzip \
  && docker-php-ext-install pdo_mysql mysqli mbstring gd iconv \
  && apt-get clean
COPY ./php.ini /usr/local/etc/php/