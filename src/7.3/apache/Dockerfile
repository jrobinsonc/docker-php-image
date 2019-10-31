FROM php:7.3-apache

RUN apt-get update; \
    apt-get install -y curl vim git wget unzip libzip-dev; \
    docker-php-ext-install zip; \
    rm -rf /var/lib/apt/lists/*;

RUN a2enmod ssl rewrite

RUN curl -sS https://getcomposer.org/installer | php -- --install-dir=/usr/local/bin --filename=composer \
    && chmod +x /usr/local/bin/composer
