FROM ubuntu:16.04

RUN apt update \
    && apt -y upgrade \
    && apt install apache2 elinks -y

RUN echo "This is a test docker" > /var/www/html/index.html

COPY httpd.conf /etc/apache2/httpd.conf

ENTRYPOINT ["elinks"]
CMD ["localhost"]

