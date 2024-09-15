FROM geobeyond/geoserver:2.20.6

USER root

COPY ./libs/sec-oauth2-openid-connect-plugin.zip /community_plugins/sec-oauth2-openid-connect-plugin.zip

RUN chown geoserveruser /community_plugins/sec-oauth2-openid-connect-plugin.zip
RUN chgrp geoserverusers /community_plugins/sec-oauth2-openid-connect-plugin.zip

RUN mkdir -p /opt/geoserver/data_dir_shared

COPY ./libs/jdom2-2.0.6.jar /usr/local/tomcat/webapps/geoserver/WEB-INF/lib/
