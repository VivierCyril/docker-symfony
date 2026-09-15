FROM php:8.4-fpm

RUN apt-get update && apt-get install -y \
    curl \
    git \
    unzip \
    libicu-dev \
    libpq-dev \
    libzip-dev \
    && curl -1sLf 'https://dl.cloudsmith.io/public/symfony/stable/setup.deb.sh' | bash \
    && apt-get install -y symfony-cli \
    && rm -rf /var/lib/apt/lists/*

RUN docker-php-ext-install pdo_mysql zip intl

COPY --from=composer:latest /usr/bin/composer /usr/bin/composer

WORKDIR /var/www/project
