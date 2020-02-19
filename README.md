# Docker PHP Image

[![Build Status](https://travis-ci.org/jrobinsonc/docker-php-image.svg?branch=master)](https://travis-ci.org/jrobinsonc/docker-php-image)

Docker image to run PHP applications based on the [official PHP image](https://github.com/docker-library/docs/blob/master/php/README.md#quick-reference), but with some added flavors.  
<https://hub.docker.com/r/jrobinsonc/php>

Why this image? Well, the difference between the original and this one is that in this image you'll find all the stuff you usually need to run PHP applications, tools like Composer and extensions like Imagick, etc.; saving you from the need of creating Dockerfiles for every new project to add all that stuff.

If you are looking for something more specific, below you can see other images designed for specific environments:

* [WordPress](https://github.com/jrobinsonc/docker-wordpress-image)
* [Laravel](https://github.com/jrobinsonc/docker-laravel-image)

## Includes

* Composer

**Image Variants**

* PHP 7.2 with Apache → `jrobinsonc/php:7.2-apache`
* PHP 7.3 with Apache → `jrobinsonc/php:7.3-apache`

## How to use

**Start the container:**

```shell
docker run \
  -p 80:80 \
  -p 443:443 \
  -v $(pwd):/var/www/html \
  jrobinsonc/php:7.3-apache
```

### More Help

* [How to install more PHP extensions](https://github.com/docker-library/docs/blob/master/php/README.md#how-to-install-more-php-extensions)
* [Running as an arbitrary user](https://github.com/docker-library/docs/blob/master/php/README.md#running-as-an-arbitrary-user)
