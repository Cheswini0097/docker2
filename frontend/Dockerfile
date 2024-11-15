FROM nginx:mainline-alpine3.20-slim
RUN rm -rf /etc/nginx/nginx.conf
COPY code /usr/share/nginx/html
COPY nginx.conf /etc/nginx/nginx.conf

