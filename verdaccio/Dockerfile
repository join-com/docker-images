# FROM verdaccio/verdaccio:5.21.1
FROM verdaccio/verdaccio:nightly-master

USER root
RUN npm install -g verdaccio-github-oauth-ui@6 && \
  npm install -g verdaccio-google-cloud && \
  npm install -g verdaccio-groups

USER $VERDACCIO_USER_UID
