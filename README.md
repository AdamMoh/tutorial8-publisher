## How many data your publlsher program will send to the message broker in one run?
The publisher will send exactly 5 data to message broker in one run, because there are 5 `publish_event` in `main.rs`.

## The url of: "amqp://guest:guest@localhost:5672" is the same as in the subscriber program, what does it mean?
The url of "amqp://guest:guest@localhost:5672" is the same as in the subscriber program, it means that the publisher and subscriber are using the same message broker, which is RabbitMQ. The publisher will send the data to the message broker, and the subscriber will receive the data from the message broker.

## Running RabbitMQ as message broker.
![RabbitMQ](/assets/ss1.png)

## Sending and processing event.
![Sending and processing event img](/assets/ss2.png)
after running subscriber and publisher, the publisher send 5 message to rabbitMQ and the subscriber will receive from rabbitMQ.

## Monitoring chart based on publisher.
![Monitoring chart](/assets/ss3.png)
After monitoring the chart, there is a relation between spikes and running the publisher. The spikes indicate the rate of message that the publisher sends to the message broker(RabbitMQ).