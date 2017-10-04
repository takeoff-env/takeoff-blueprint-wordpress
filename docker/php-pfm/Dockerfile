FROM php:7.0.6-fpm-alpine

RUN docker-php-ext-install -j$(grep -c ^processor /proc/cpuinfo 2>/dev/null || 1) iconv gd mbstring fileinfo curl xmlreader xmlwriter spl ftp mysqli

VOLUME /home/wordpress/wordpress
