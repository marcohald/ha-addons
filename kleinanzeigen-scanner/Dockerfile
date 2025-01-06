# https://developers.home-assistant.io/docs/add-ons/configuration#add-on-dockerfile
ARG BUILD_FROM
FROM $BUILD_FROM

# Install build dependencies required for pycurl
RUN apk update && apk add --no-cache \
    build-base \
    libcurl \
    libcurl-dev \
    python3-dev \
    py3-pip \
    && pip install --no-cache-dir pycurl \
    && apk del build-base python3-dev


# Copy root filesystem
COPY rootfs /
#RUN git clone https://github.com/marcohald/Kleinanzeigen-Telegram-Bot.git /opt/kleinanzeigen-scanner/
RUN find /opt/
RUN pip install -r /opt/kleinanzeigen-scanner/requirements.txt