FROM php:fpm
ADD https://getcomposer.org/installer .
RUN apt-get update && apt-get install unzip
RUN php installer
ADD composer.json .
RUN php composer.phar install
ADD index.php .
