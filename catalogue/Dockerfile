FROM node:18
EXPOSE 8080
RUN groupadd roboshop && useradd -aG roboshop roboshop
WORKDIR /opt/server
ENV MONGO=true
COPY package.json /opt/server/
RUN 
COPY server.js /opt/server/
COPY catalogue.js /opt/server/
RUN npm install
CMD ["node", "server.js"]