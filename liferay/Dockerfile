FROM liferay/portal:7.4.3.100-ga100

USER root

ENV LD_LIBRARY_PATH=/lib64

RUN apt-get update -y && apt-get install -y mysql-client

ADD override /mnt/liferay

RUN chown -R liferay:liferay /mnt/liferay