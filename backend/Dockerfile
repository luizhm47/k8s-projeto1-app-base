FROM php:apache

WORKDIR /var/www/html

COPY *.php ./

RUN apt update && apt install -y libpng-dev \
    && docker-php-ext-install mysqli \
    && docker-php-ext-install pdo_mysql

EXPOSE 80
