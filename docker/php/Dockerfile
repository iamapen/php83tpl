FROM php:8.3.9-cli

# Install Xdebug
RUN pecl install xdebug \
    && docker-php-ext-enable xdebug

CMD ["php", "-a"]
