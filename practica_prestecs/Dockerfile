FROM php:8.2-apache

RUN docker-php-ext-install mysqli

# Copiar el fitxer PHP al contenidor
COPY index.php /var/www/html/

# Opcional però recomanat per a dev: errors visibles
RUN { \
  echo "display_errors=On"; \
  echo "display_startup_errors=On"; \
  echo "error_reporting=E_ALL"; \
} > /usr/local/etc/php/conf.d/dev-errors.ini
