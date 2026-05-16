FROM python:3.10.20-alpine
WORKDIR /opt/server
ENV CART_HOST="cart" \
    CART_PORT="8080" \
    USER_HOST="user" \
    USER_PORT="8080" \
    AMQP_HOST="rabbitmq"
COPY *.py .
COPY *.ini .
COPY *.txt .
RUN pip3 install --no-cache-dir --prefix=/install -r requirements.txt
#RUN pip3 install -r requirements.txt
CMD ["uwsgi", "--ini", "payment.ini"]
