# Docker PHP Image

[![Build Status](https://travis-ci.org/jrobinsonc/docker-php-image.svg?branch=master)](https://travis-ci.org/jrobinsonc/docker-php-image)

Docker image to run PHP applications.  
<https://hub.docker.com/r/jrobinsonc/php>

## Includes

* Composer

## How to use

This image is an environment designed to perfectly run a PHP application.

**Start the container:**

```shell
docker run -d \
  --name app \
  -p 80:80 \
  -p 443:443 \
  -v $(pwd):/var/www/html \
  jrobinsonc/php:7.3-apache
```
