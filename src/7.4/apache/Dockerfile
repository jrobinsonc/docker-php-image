FROM php:7.4-apache

RUN set -ex; \
    apt-get update; \
    apt-get install -y --no-install-recommends \
      curl \
      vim \
      git \
      wget \
      unzip \
      libzip-dev \
    ; \
    rm -rf /var/lib/apt/lists/*;

RUN set -ex; \
    docker-php-ext-install \
      zip \
    ;

RUN curl -sS https://getcomposer.org/installer | php -- --install-dir=/usr/local/bin --filename=composer \
    && chmod +x /usr/local/bin/composer
