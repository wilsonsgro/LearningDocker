FROM alastairhm/alpine-lighttpd:latest
MAINTAINER Alastair Montgomery <alastair@montgomery.me.uk>

ARG PHP_UPSTREAM=php-fpm
RUN apk update && \
    apk upgrade && \
    apk add --update bind && \
    apk add --update bash && \
    apk add --update wget && \
    apk add --update curl && \
    apk add --update nano && \
    apk add --update nmap && \
    apk add --update busybox 


ADD lighttpd.conf /etc/lighttpd/lighttpd.conf
COPY sites/*.conf /etc/lighttpd/conf-enabled/ 

RUN mkdir -p /run/lighttpd/
RUN chown www-data. /run/lighttpd/

EXPOSE 80 443
VOLUME /var/www/test.local
                    
CMD php-fpm -D && lighttpd -D -f /etc/lighttpd/lighttpd.conf