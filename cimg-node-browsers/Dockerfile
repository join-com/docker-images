ARG CIMG_NODE_VERSION=14.19.0

FROM cimg/node:${CIMG_NODE_VERSION}-browsers

# hadolint ignore=DL3004
RUN   sudo apt-get update && \
      sudo apt-get install -y --no-install-recommends --no-upgrade \
      libgconf-2-4 \
      && \
	sudo rm -rf /var/lib/apt/lists/*
