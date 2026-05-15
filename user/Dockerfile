From node:20
WORKDIR /opt/server
ENV REDIS_URL="redis" \
    MONGO_URL="mongodb" \
    MONGO="true"
COPY *.json .
COPY *.js .
RUN npm install
CMD ["node","server.js"]

 