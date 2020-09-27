# docker-jenkins

## Run

```bash
docker run --rm --name myjenkins -d \
    -p 8080:8080 -p 50000:50000 \
    -v /data/jenkins_home:/var/jenkins_home \
    -u 0 \
    jenkins:alpine
```
