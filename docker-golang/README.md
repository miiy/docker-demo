# docker-golang

## Build

```bash
docker build -t docker-go:1.0 --build-arg GO_VERSION=1.15 .

docker build . -t docker-go
```

## Run

```bash
docker run --rm --name mygolang -d \
    -p 8080:8080 \
    docker-go:1.0
```

## sh

```bash
docker exec -it [CONTAINER ID] sh
```
