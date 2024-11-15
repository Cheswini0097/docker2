FROM nginx
RUN rm -rf /usr/share/nginx/html/*
COPY code /usr/share/nginx/html
COPY expense.conf /etc/nginx/nginx.conf/expense.conf