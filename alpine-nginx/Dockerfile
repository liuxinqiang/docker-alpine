FROM juehai/alpine-base:1.0.0
MAINTAINER Juehai (https://juehai.com)

# Install nginx
RUN echo "https://dl-4.alpinelinux.org/alpine/v3.16/main" >> /etc/apk/repositories && \
    apk add --update nginx && \
    rm -rf /var/cache/apk/* && \
    chown -R nginx:www-data /var/lib/nginx

# Add the files
ADD root /

# Expose the ports for nginx
EXPOSE 80 443
