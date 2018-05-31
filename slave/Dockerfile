FROM centos:centos7
RUN yum install bind bind-utils -y
COPY ./named.conf /etc/named.conf
RUN chown root:named /etc/named.conf
CMD /sbin/init