# https://developers.home-assistant.io/docs/apps/configuration#app-dockerfile
ARG BUILD_FROM=ghcr.io/home-assistant/base:3.23
FROM ${BUILD_FROM}

# Install requirements for app
RUN \
  apk add --no-cache \
    python3 py3-pip git build-base

RUN pip install --break-system-packages "git+https://github.com/google/liblc3.git@v1.1.3" \
    sendspin_auracast==0.2.2

# Copy root filesystem
COPY rootfs /

LABEL \
    org.opencontainers.image.title="Home Assistant App: Sendspin Auracast" \
    org.opencontainers.image.description="Sendspin Auracast app for Home Assistant." \
    org.opencontainers.image.source="https://github.com/Yagoor/app_sendspin_auracast" \
    org.opencontainers.image.licenses="Apache License 2.0"
