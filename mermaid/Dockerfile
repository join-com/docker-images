FROM ghcr.io/mermaid-js/mermaid-live-editor as source

FROM nginxinc/nginx-unprivileged:1.23.3-alpine

RUN rm /etc/nginx/conf.d/default.conf

COPY nginx.conf /etc/nginx/nginx.conf
COPY --from=source /usr/share/nginx/html /usr/share/nginx/html

USER 101
EXPOSE 8080
CMD ["nginx", "-g", "daemon off;"]
