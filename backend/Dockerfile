FROM node:20
EXPOSE 8080
RUN mkdir /opt/server
WORKDIR /opt/server
COPY package.json .
COPY *.js .
RUN npm install
ENV DB_HOST="localhost"
CMD [ "node", "index.js" ]