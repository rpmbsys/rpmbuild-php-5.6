ARG os=8.10.20240528
ARG image=devbase
FROM ghcr.io/rpmbsys/php56build:${os}-${image}

LABEL org.opencontainers.image.source=https://github.com/rpmbsys/rpmbuild-php-5.6

RUN curl -sSL https://getcomposer.org/installer | php -- --install-dir=/usr/local/bin --filename=composer
