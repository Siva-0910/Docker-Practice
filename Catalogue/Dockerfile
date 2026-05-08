FROM node:20
WORKDIR /opt/server
RUN npm install .
COPY *.js .
COPY package.json /opt/server
ENV MONGO_URL="mongodb://mongodb:27017/catalogue" \
    MONGO="true"
CMD ["node","server.js"]
