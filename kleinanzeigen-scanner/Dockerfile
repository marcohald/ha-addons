# https://developers.home-assistant.io/docs/add-ons/configuration#add-on-dockerfile
ARG BUILD_FROM
FROM $BUILD_FROM


# Copy root filesystem
COPY rootfs /
RUN git clone https://github.com/marcohald/Kleinanzeigen-Telegram-Bot.git /opt/kleinanzeigen-scanner/
RUN find /opt/
RUN pip install -r /opt/kleinanzeigen-scanner/requirements.txt