FROM php:8.3.9-cli

# Install Xdebug
RUN pecl install xdebug \
    && docker-php-ext-enable xdebug

# Install composer
RUN curl -sS https://getcomposer.org/installer | php -- --version=2.7.8 \
    && mv composer.phar /usr/local/bin/composer

CMD ["php", "-a"]
