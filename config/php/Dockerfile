FROM php:7.4-apache

RUN apt-get update && apt-get install -y \
    libonig-dev \
  && docker-php-ext-install pdo_mysql mysqli


#COPY ./php.ini /usr/local/etc/php/


#PHP-debug
RUN pecl install xdebug \
    && docker-php-ext-enable xdebug



# Xdebug の設定ファイルを Docker コンテナに配置
#COPY ./20-xdebug.ini /usr/local/etc/php/conf.d/20-xdebug.ini
