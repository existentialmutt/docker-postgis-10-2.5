# Multiplatform-compatible Dockerfile for building Postgres w/ PostGIS

This repository targets Postgres 10 with PostGIS 2.5.  The docker image is published on docker hub as `existentialmutt/postgis:10-2.5`

To build for amd64 (Intel processors) and arm64 (Apple Silicon) run
```
docker buildx build --platform=linux/amd64,linux/arm64 -t existentialmutt/postgis:10-2.5 . --push
```

Based on the official PostGIS Docker images.  See the [official repo](https://github.com/postgis/docker-postgis) for more information.
