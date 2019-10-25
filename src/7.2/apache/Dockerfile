FROM php:7.2-apache

RUN apt-get update; \
    apt-get install -y curl vim git wget unzip; \
    rm -rf /var/lib/apt/lists/*;

RUN curl -sS https://getcomposer.org/installer | php -- --install-dir=/usr/local/bin --filename=composer \
    && chmod +x /usr/local/bin/composer
