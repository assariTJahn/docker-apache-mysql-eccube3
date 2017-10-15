FROM php:7.1-apache
RUN apt-get update && apt-get install -y \
       apt-utils \
       zlib1g-dev \
       libmcrypt-dev \
    && apt-get clean \
    && rm -rf /var/lib/apt/lists/*

RUN docker-php-source extract \
    && docker-php-ext-install pdo pdo_mysql \
    && docker-php-ext-install zip \
    && docker-php-ext-install opcache \
    && docker-php-ext-install mcrypt
    

RUN curl -sS https://getcomposer.org/installer | php
RUN mv composer.phar /usr/local/bin/composer

RUN pecl install apcu
RUN echo "extension=apcu.so" > /usr/local/etc/php/conf.d/apcu.ini
RUN a2enmod rewrite
RUN service apache2 restart