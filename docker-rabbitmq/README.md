# docker-rabbitmq

## Build

```bash
docker build -t docker-rabbitmq:1.0 --build-arg RABBIMQ_VERSION=3.8 .
```

## Run

```bash
docker run --rm --name myabbitmq -d \
    -e RABBITMQ_DEFAULT_USER=admin -e RABBITMQ_DEFAULT_PASS=123456 \
    -p 4369:4369 -p 5671:5671 -p 5672:5672 -p 15672:15672 \
    -v /data/rabbitmq:/var/lib/rabbitmq \
    docker-rabbitmq:1.0
```

## Management Plugin

visiting http://localhost:15672/

Username: admin

Password: 123456