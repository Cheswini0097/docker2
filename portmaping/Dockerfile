FROM ubuntu:latest
RUN sudo su -
RUN apt-get install nginx -y
WORKDIR /nginx
EXPOSE 80
CMD ["nginx", "-g", "daemon off;"]