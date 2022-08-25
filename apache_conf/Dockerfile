FROM centos:7
RUN yum -y update
RUN yum -y install httpd httpd-devel gcc* make vim less
CMD ["/usr/sbin/apachectl","-DFOREGROUND"]
