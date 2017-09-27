FROM centos

MAINTAINER salamander 1906747819@qq.com


RUN yum install -y pcre-devel wget net-tools gcc zlib zlib-devel make openssl-devel
# 添加文件
RUN wget http://nginx.org/download/nginx-1.12.1.tar.gz
RUN tar -zxvf nginx-1.12.1.tar.gz
RUN mkdir -p /usr/local/nginx
RUN cd nginx-1.12.1 && ./configure --prefix=/usr/local/nginx && make && make install
ADD nginx.conf /usr/local/nginx/conf/nginx.conf


# Expose ports
EXPOSE 80
EXPOSE 443


CMD ["/usr/local/nginx/sbin/nginx"]