FROM centos:7

MAINTAINER mango <1192297699@qq.com>

USER root
RUN yum update -y 
RUN   yum -y install gcc zlib zlib-devel pcre-devel openssl openssl-devel

RUN mkdir -p /usr/local/nginx
RUN wget http://nginx.org/download/nginx-1.13.7.tar.gz -P /usr/local/
RUN tar -xvf /usr/local/nginx-1.13.7.tar.gz -C /usr/local/
RUN mv /usr/local/nginx-1.13.7 /usr/local/nginx
RUN /usr/local/nginx/configure
RUN make && make install

CMD ["/bin/bash"]
