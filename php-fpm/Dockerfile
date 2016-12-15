FROM php:fpm
RUN docker-php-ext-enable opcache
RUN apt-get update && apt-get install php5-mysql -y 
RUN docker-php-ext-install pdo pdo_mysql
