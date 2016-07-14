FROM php:5.5-fpm

# Install selected extensions and other stuff
RUN apt-get update \
    && apt-get -y --no-install-recommends install php5-fpm php5-mysql php5-gd php5-imagick libcurl3 php5-curl php5-mcrypt libpng-dev zlib1g-dev libmcrypt-dev \
    && apt-get clean; rm -rf /var/lib/apt/lists/* /tmp/* /var/tmp/* /usr/share/doc/*


RUN docker-php-ext-install pdo pdo_mysql gd
RUN docker-php-ext-install mcrypt

WORKDIR "/var/www/test"
