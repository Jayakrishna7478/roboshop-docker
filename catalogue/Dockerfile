FROM node:14
EXPOSE 8080
RUN addgroup -S roboshop && adduser -S roboshop -G roboshop
WORKDIR /opt/server
COPY package.js /opt/server/
RUN npm install
COPY server.js /opt/server/
CMD [ "node", "server.js" ]