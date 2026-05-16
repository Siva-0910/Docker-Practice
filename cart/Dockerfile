FROM node:20-alpine3.21
WORKDIR /opt/server
COPY *.js .
COPY package.json /opt/server
#RUN npm install \
RUN npm install -g npm@11.14.1
ENV REDIS_HOST="redis" \
    CATALOGUE_HOST="catalogue" \
    CATALOGUE_PORT="8080"

CMD ["node","server.js"]