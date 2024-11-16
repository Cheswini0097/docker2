FROM node:20
EXPOSE 8080
ENV DB_HOST="localhost"
RUN mkdir /opt/server
WORKDIR /opt/server
COPY package.json
COPY *.js .
CMD [ "node","index.js" ]
