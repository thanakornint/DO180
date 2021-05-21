FROM ubi7/ubi:7.7
MAINTAINER Thanakorn <thanakorn.int@gmail.com>
LABEL description="A custom Apache container based on UBI7"
RUN yum install -y httpd && \
    yum clean all
RUN echo "Hello from Dockerfile" > /var/www/html/index.html
EXPOSE 80
CMD ["httpd", "-D", "FOREGROUND"]
