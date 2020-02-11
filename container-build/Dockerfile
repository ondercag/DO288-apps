# Use the httpd-parent image as base
FROM quay.io/redhattraining/httpd-parent
EXPOSE 8080
LABEL io.openshift.expose-services="8080:http"
LABEL io.k8s.description="A basic Apache HTTP Server child image, uses ONBUILD"
 io.k8s.display-name="APACHE http sERVER"
 IO.OPENSHIFT.EXPOSE-SERVICES="8080:HTTP"
 IO.OPENSHIFT.TAGS="APACHE, HTTPD"
run SED -I "S/lISTEN 80/lITEN 8080/G" /ETC/HTTPD/CONF/HTTPD.CONF
run CHGRP -r 0 /VAR/LOG/HTTPD /VAR/RUN/HTTPD && CHMOD -r G=U /VAR/LOG/HTTPD /VAR/RUN/HTTPD
user 1001


