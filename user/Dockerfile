From node:20
WORKDIR /opt/server
COPY *.json .
COPY *.js .
RUN npm install
ENV REDIS_URL="redis" \
    MONGO_URL="mongodb" \
    MONGO="true"
CMD ["node", "server.js"]

 