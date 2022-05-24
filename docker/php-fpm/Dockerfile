FROM php:8.1.6-fpm-alpine

WORKDIR /var/www/html
RUN apk update && apk add composer php8-tokenizer php8-dom php8-xml php8-xmlwriter php8-fileinfo \
&& composer create-project --prefer-dist laravel/laravel laravel
WORKDIR laravel
RUN composer install \
&& php artisan key:generate