FROM ubuntu:14.04
RUN apt-get update

ENV DEBIAN_FRONTEND noninteractive

RUN apt-get install -y \
    git \
    curl \
    php5-cli \
    php5-json \
    php5-intl \
    php5-mysql \
    php5-sqlite

RUN mkdir -p /usr/local/bin
RUN curl -LsS https://symfony.com/installer -o /usr/local/bin/symfony
RUN chmod a+x /usr/local/bin/symfony

#Installation of composer
RUN curl -sS https://getcomposer.org/installer | sudo php -- --install-dir=/usr/local/bin --filename=composer
