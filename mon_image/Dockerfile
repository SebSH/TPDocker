FROM php:7.2-apache

RUN docker-php-ext-install pdo pdo_mysql
COPY my-php-files/ /var/www/html/
RUN useradd user && usermod -g root user &&\
sed -i s/DocumentRoot.*/DocumentRoot\ user/
