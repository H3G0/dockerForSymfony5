## TODO fix DB WAIT 

FROM zolweb/php-fpm:7.3.16

RUN apk --update --no-cache add git

RUN docker-php-ext-install pdo_mysql

COPY --from=composer /usr/bin/composer /usr/bin/composer

WORKDIR /var/www

CMD composer install ;  php 

EXPOSE 9000

