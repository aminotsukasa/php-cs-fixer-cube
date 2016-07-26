 FROM php:7.0-cli
RUN set -x && \
    apt-get update && \
    apt-get -y install zip git php-pclzip && \
    curl -sS https://getcomposer.org/installer | php -- --install-dir=/usr/bin && \
    mv /usr/bin/composer.phar /usr/bin/composer && \
    composer global require fabpot/php-cs-fixer && \
    ln -s /root/.composer/vendor/bin/php-cs-fixer /usr/bin
