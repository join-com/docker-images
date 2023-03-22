FROM node:lts-alpine as builder

RUN mkdir -p /verdaccio/plugins \
  && cd /verdaccio/plugins \
  && npm install --global-style --no-bin-links --omit=optional @xlts.dev/verdaccio-prometheus-middleware@x.y.z


FROM verdaccio/verdaccio:5.21.1

USER root
RUN npm install -g verdaccio-github-oauth-ui@6 && \
  npm install -g verdaccio-google-cloud

COPY --chown=$VERDACCIO_USER_UID:root --from=builder \
  /verdaccio/plugins/node_modules/@xlts.dev/verdaccio-prometheus-middleware \
  /verdaccio/plugins/verdaccio-metrics

USER $VERDACCIO_USER_UID
