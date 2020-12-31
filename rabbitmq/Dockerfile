FROM rabbitmq:3.8-management
COPY . /rabbitmq
WORKDIR /rabbitmq
RUN rabbitmq-plugins enable --offline rabbitmq_mqtt rabbitmq_federation_management rabbitmq_stomp
