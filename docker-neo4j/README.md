# docker-neo4j

## Run

```bash
docker run --rm --name myneo4j -d \
    --env=NEO4J_AUTH=neo4j/123456 \
    -p 7474:7474 -p 7687:7687 \
    -v /data/neo4j/data:/data \
    neo4j
```
