FROM mongo:7.0
COPY *.js /docker-entrypoint-initdb.d
CMD ["mongod", "--bind_ip", "0.0.0.0"]

