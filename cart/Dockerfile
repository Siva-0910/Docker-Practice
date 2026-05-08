FROM node:20
WORKDIR /opt/server
COPY *.js .
COPY package.json /opt/server
ENV REDIS_HOST="redis" \
    CATALOGUE_HOST="catalogue" \
    CATALOGUE_PORT="8080"
RUN npm install
CMD ["node","server.js"]