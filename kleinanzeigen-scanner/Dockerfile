# https://developers.home-assistant.io/docs/add-ons/configuration#add-on-dockerfile
ARG BUILD_FROM
FROM $BUILD_FROM


# Copy root filesystem
COPY rootfs /

RUN find /opt/
RUN pip install -r /opt/kleinanzeigen-scanner/requirements.txt