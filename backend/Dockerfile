FROM node:20
EXPOSE 8080
RUN mkdir /opt/server
WORKDIR /opt/server
COPY package.json .
COPY *.js .
RUN npm install
ENV DB_HOST="mysqlcont"
CMD [ "node", "index.js" ]