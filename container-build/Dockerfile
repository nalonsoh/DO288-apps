# Use the httpd-parent image as base
FROM quay.io/redhattraining/httpd-parent

RUN chgrp 0 /var/log/httpd /var/run/httpd \
 && chmod g=u /var/log/httpd /var/run/httpd \
 && seed -i "s/Listen 80/Listen/8080/g" /etc/httpd/conf/httpd.conf

USER 1001
