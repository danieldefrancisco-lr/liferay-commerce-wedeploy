FROM liferay/commerce:1.0.1

RUN mkdir -p /etc/liferay/mount/deploy
RUN mkdir -p /etc/liferay/mount/files
RUN mkdir -p /etc/liferay/mount/files/osgi/configs
ADD ./deploy /etc/liferay/mount/deploy
ADD portal-ext.properties /etc/liferay/mount/files
ADD ./configs /etc/liferay/mount/files/osgi/configs
USER root
RUN chown liferay:liferay -R /etc/liferay/mount/
USER liferay