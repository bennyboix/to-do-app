

FROM php:8.2-apache


RUN docker-php-ext-install mysqli pdo pdo_mysql


RUN mv "$PHP_INI_DIR/php.ini-production" "$PHP_INI_DIR/php.ini"

COPY . /var/www/html

USER www-data

EXPOSE 80