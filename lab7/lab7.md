## video
https://www.youtube.com/watch?v=kWazFcjSpM4


## analysis analysis of the RabbitMQ configuration issues

- rabbitmq is a stateful application
- the implication of running RabbitMQ without persistent storage is that if the pod is deleted or restarted, all the messages in the queue will be lost.
- the rabbitmq service is not available when the pod is deleted or restarted.
- using persistent storage can solve the issue of message loss when the pod is deleted or restarted.
- using azure service bus can solve the issue of rabbitmq service not available when the pod is deleted or restarted.