# Springboot-Rabbitmq-sample
Using RabbitMQ as a Publisher and Consumer model

## Rabbit MQ Notes
----------------------------------
1. Rabbit MQ is a message broker that implements Advanced message queuing protocol.
2. The AMQP standardizes messages using Producer, broker and consumer.
3. In a practical scenario we have multiple queues used to handle different requests and multiple consumers. Therefore in order to indentify the queue to which a particular record needs to
be forwared we use a Routing Key that is passed on to the Exchange.

Install RabbitMQ in windows :
-----------------------------
1. Download and install Rabbit MQ: https://www.rabbitmq.com/install-windows.html#chocolatey
2. As a pre-requisite for RabbitMQ we need Erlang OTP to be downloaded. (Download: https://www.rabbitmq.com/which-erlang.html)
3. Install both RabbitMQ and Erlang OTP as administrator
3. Go to RabbitMQ Server install Directory C:\Program Files\RabbitMQ Server\rabbitmq_server-3.8.3\sbin
4. Run command: rabbitmq-plugins enable rabbitmq_management
5. rabbitmq-service.bat start  (RUN as administrator)
6. Open browser and enter http://localhost:15672/ to redirect to RabbitMQ Dashboard
7. Also we can Open it with IP Address http://127.0.0.1:15672
8. Login page default username and password is guest 
9. After successfully login you should see RabbitMQ Home page

