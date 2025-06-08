FROM php:8.2-fpm

# パッケージ
RUN apt-get update && apt-get install -y \
    git zip unzip curl libzip-dev \
    && docker-php-ext-install zip pdo pdo_mysql

# Composer
COPY --from=composer:latest /usr/bin/composer /usr/bin/composer

WORKDIR /var/www
