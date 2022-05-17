FROM wordpress:php8.0-fpm-alpine

COPY cmd.sh /usr/local/bin

WORKDIR /app

RUN apk add curl tar && \
    curl https://wordpress.org/latest.tar.gz > wordpress.tar.gz && \
    tar -xzf wordpress.tar.gz && cd /app/wordpress && \
    rm -rf wordpress.tar.gz && \ 
    mv wp-config-sample.php wp-config.php

WORKDIR /app/wordpress

CMD [ "cmd.sh" ]



