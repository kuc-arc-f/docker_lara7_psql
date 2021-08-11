FROM php:7.3-fpm
RUN apt-get update && apt-get install -y \
   vim \
   zip \
   unzip \
   iputils-ping \
   git
RUN set -ex apk --no-cache add postgresql-dev libpq-dev && \
    apt-get update && apt-get install -y \
    less \
    libpq-dev \
    postgresql \
    && docker-php-ext-install \
    mbstring \
    pdo \
    pdo_pgsql \
    pgsql
