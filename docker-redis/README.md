# docker-redis

## Run

```bash
$ docker run --rm --name myredis --network backend -d \
    -p 6379:6379 \
    -v /data/config/redis/redis.conf:/usr/local/etc/redis/redis.conf \
    -v /data/redis:/data \
    redis:6.0-alpine

$ docker inspect [CONTAINER ID]
$ docker run -it --network backend --rm redis:6.0-alpine redis-cli -h [IP]
```

