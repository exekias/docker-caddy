# docker-caddy

Docker image for [Caddy](http://caddyserver.com) server

This image downloads latest Caddy version. By default it offers the following Caddyfile:

```
0.0.0.0
log
browse
```

## Paths

You can use a custom Caddyfile, image uses `/Caddyfile` when running the server:

```
docker run -t -v ./MyCaddyfile:/Caddyfile exekias/caddy
```

## Ports

By default ports 80, 443 and 2014 are exposed, you can publish them in the host:

```
docker run -t -p 80:80 exekias/caddy
```
