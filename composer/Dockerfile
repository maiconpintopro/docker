FROM composer as composer

FROM php:8.1-apache as server
COPY --from=composer /usr/bin/composer /usr/bin/composer

RUN apt-get update && apt-get install -y zip unzip \
    libicu-dev \
    && docker-php-ext-install intl

WORKDIR /app

ENTRYPOINT ["composer", "create-project", "cakephp/app", "--no-interaction"]