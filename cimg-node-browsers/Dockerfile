ARG CIMG_NODE_VERSION=18.16.0

FROM cimg/node:${CIMG_NODE_VERSION}-browsers

# hadolint ignore=DL3004
RUN   sudo apt-get update && \
      sudo apt-get install -y --no-install-recommends --no-upgrade \
      libgconf-2-4 libvulkan1 libu2f-udev

ENV CHROME_VERSION 113.0.5672.126
ENV CHROME_PATH /opt/google/chrome/google-chrome

# install Chrome browser
# hadolint ignore=DL3004
RUN   sudo wget -O /usr/src/google-chrome-stable_current_amd64.deb "http://dl.google.com/linux/chrome/deb/pool/main/g/google-chrome-stable/google-chrome-stable_${CHROME_VERSION}-1_amd64.deb" && \
      sudo dpkg -i /usr/src/google-chrome-stable_current_amd64.deb && \
      sudo apt-get install -f -y && \
      sudo rm -f /usr/src/google-chrome-stable_current_amd64.deb && \
      sudo rm -rf /var/lib/apt/lists/*
