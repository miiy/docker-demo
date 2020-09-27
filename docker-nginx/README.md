# docker-nginx

## Run

```bash
docker run --rm --name mynginx -d \
    -p 80:80 -p 443:443 \
    -v /data/www:/data/www/:ro \
    -v /data/config/config/nginx/nginx.conf:/etc/nginx/nginx.conf:ro \
    -v /data/config/nginx/conf.d/:/etc/nginx/conf.d:ro \
    -v /data/log/nginx/:/var/log/nginx:rw \
    nginx:stable-alpine
```