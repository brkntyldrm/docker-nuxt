FROM wordpress:php8.0-fpm-alpine

COPY cmd.sh /usr/local/bin

WORKDIR /app/wordpress/wp-content/themes/

RUN mkdir tailpress

COPY tailpress tailpress

WORKDIR /app/wordpress

# CMD [ "cmd.sh" ]




