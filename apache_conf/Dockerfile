FROM centos:7
RUN yum -y update
RUN yum -y install httpd httpd-devel gcc* make vim less
CMD ["/usr/sbin/apachectl","-DFOREGROUND"]
RUN touch /etc/httpd/conf.d/hoge.example.com.conf
RUN touch /etc/httpd/conf.d/fuga.example.com.conf
RUN mkdir -p /var/www/vhosts/public_html/hoge.example.com
RUN mkdir -p /var/www/vhosts/public_html/fuga.example.com
RUN chown -R apache:apache /var/www/vhosts/public_html/hoge.example.com
RUN chown -R apache:apache /var/www/vhosts/public_html/fuga.example.com
RUN touch /var/www/vhosts/public_html/hoge.example.com/index.html
RUN touch /var/www/vhosts/public_html/fuga.example.com/index.html
RUN echo 'hoge.example.com' >> /var/www/vhosts/public_html/hoge.example.com/index.html
RUN echo 'fuga.example.com' >> /var/www/vhosts/public_html/fuga.example.com/index.html
