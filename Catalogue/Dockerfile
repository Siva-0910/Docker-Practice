FROM node:20-alpine3.21
WORKDIR /opt/server
COPY *.js .
COPY package.json /opt/server
RUN npm install
ENV MONGO_URL="mongodb://mongodb:27017/catalogue" \
    MONGO="true"
CMD ["node","server.js"]
