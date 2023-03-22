FROM verdaccio/verdaccio:5.21.1

USER root
RUN npm install -g verdaccio-github-oauth-ui@6 && \
  npm install -g --no-bin-links --omit=optional @xlts.dev/verdaccio-prometheus-middleware@2.0.2 && \
  npm install -g verdaccio@latest

USER $VERDACCIO_USER_UID
