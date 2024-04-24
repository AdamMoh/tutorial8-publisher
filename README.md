## How many data your publlsher program will send to the message broker in one run?
The publisher will send exactly 5 data to message broker in one run, because there are 5 `publish_event` in `main.rs`.

## The url of: "amqp://guest:guest@localhost:5672" is the same as in the subscriber program, what does it mean?
The url of "amqp://guest:guest@localhost:5672" is the same as in the subscriber program, it means that the publisher and subscriber are using the same message broker, which is RabbitMQ. The publisher will send the data to the message broker, and the subscriber will receive the data from the message broker.

## Running RabbitMQ as message broker.
![RabbitMQ](/assets/ss1.png)