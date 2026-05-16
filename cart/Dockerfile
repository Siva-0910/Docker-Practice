FROM node:20-alpine3.21
WORKDIR /opt/server
COPY *.js .
COPY package.json /opt/server
RUN npm install
ENV REDIS_HOST="redis" \
    CATALOGUE_HOST="catalogue" \
    CATALOGUE_PORT="8080"

CMD ["node","server.js"]