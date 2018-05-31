FROM centos/systemd
RUN yum install bind bind-utils -y
COPY ./named.conf /etc/named.conf
COPY ./hal29.ac.jp.zone /var/named/hal29.ac.jp.zone
RUN chown root:named /etc/named.conf & chown root:named /var/named/hal29.ac.jp.zone
RUN systemctl enable named
CMD /sbin/init
