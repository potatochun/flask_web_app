FROM rabbitmq:3-management

COPY ./rabbitmq/rabbitmq.conf /etc/rabbitmq/rabbitmq.conf
COPY ./rabbitmq/definitions.json /etc/rabbitmq/definitions.json

RUN rabbitmq-plugins enable rabbitmq_management
