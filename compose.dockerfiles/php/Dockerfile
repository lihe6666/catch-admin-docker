FROM php:fpm
MAINTAINER cow "lihe6666@163.com"

ENV TZ=Asia/Shanghai
RUN ln -snf /usr/share/zoneinfo/$TZ /etc/localtime && echo $TZ > /etc/timezone

RUN mv "$PHP_INI_DIR/php.ini-development" "$PHP_INI_DIR/php.ini"

#RUN pecl install redis && docker-php-ext-enable redis \
#	&& pecl install xdebug && docker-php-ext-enable xdebug
#
#RUN php -r "copy('https://install.phpcomposer.com/installer', 'composer-setup.php');" \
#    && php composer-setup.php \
#    && php -r "unlink('composer-setup.php');" \
#    && mv composer.phar /usr/local/bin/composer \
#    && composer config -g repo.packagist composer https://packagist.phpcomposer.com \
#	&& composer install
