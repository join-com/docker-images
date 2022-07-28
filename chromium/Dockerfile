FROM debian:bullseye-slim

ARG CHROMIUM_VERSION=103.0.5060.134
ENV DEBIAN_FRONTEND noninteractive
ENV RD_PORT 9222

# hadolint ignore=DL3008
RUN apt-get update \
    && apt-get install --no-install-recommends -qy \
        dumb-init \
        fontconfig \
        chromium=${CHROMIUM_VERSION}\* \
    && rm -rf /var/lib/apt/lists/* \
    && groupadd chromium \
    && useradd --create-home --gid chromium chromium \
    && chown --recursive chromium:chromium /home/chromium/

VOLUME ["/home/chromium/.fonts"]

COPY --chown=chromium:chromium entrypoint.sh /home/chromium/

USER chromium
EXPOSE ${RD_PORT}
ENTRYPOINT ["dumb-init", "--", "/bin/sh", "/home/chromium/entrypoint.sh"]
