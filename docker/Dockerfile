FROM php:7.4-apache

COPY ./docker/site.conf /etc/apache2/sites-available/000-default.conf

RUN a2enmod rewrite
RUN a2ensite 000-default.conf
RUN chown -R www-data:www-data /var/www
RUN service apache2 restart

