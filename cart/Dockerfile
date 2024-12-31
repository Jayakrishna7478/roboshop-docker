FROM node:node:18.19.1-alpine3.19
EXPOSE 8080
WORKDIR /opt/server
ENV MONGO=true
COPY package.json /opt/server/
RUN chown roboshop:roboshop /opt/server
USER roboshop
COPY server.js /opt/server/
COPY package.js /opt/server/
RUN npm install
CMD ["node", "server.js"]