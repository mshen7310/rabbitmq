# rabbitmq
A customized RabbitMQ image that enables various plugins by default and pre-installed rabbitmqadmin and python. 

# Usage:

## Build

```
git clone https://github.com/mshen7310/rabbitmq.git
cd rabbitmq
docker build -t mshen7310/rabbitmq .
```

## Run

```
docker run -d --hostname rabbit --name rabbit -p 15674:15674 -p 15672:15672 -p 4369:4369 -p 5671:5671 -p 5672:5672 -p 25672:25672  mshen7310/rabbitmq:latest

```

## Setup shovel

```
docker exec rabbit init
```

