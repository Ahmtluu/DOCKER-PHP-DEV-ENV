FROM php:8.2-fpm

RUN apt-get update
RUN apt-get upgrade -y

RUN apt-get install libzip-dev -y
RUN apt-get install zip unzip -y
RUN apt-get install git -y
RUN apt-get install curl -y


RUN docker-php-ext-install zip  
RUN docker-php-ext-install mysqli 
RUN docker-php-ext-install bcmath 
RUN docker-php-ext-install ctype 
RUN docker-php-ext-install fileinfo 
RUN docker-php-ext-install pdo 

RUN curl -sS https://getcomposer.org/installer | php -- --install-dir=/usr/local/bin --filename=composer
#RUN chown -R www-data:www:data /var/www/html

