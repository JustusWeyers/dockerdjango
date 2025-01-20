# dockerdjango

Testing some stuff

# Docker

## buildx

Some basic buildx commands are:
```
docker buildx ls
```
```
docker buildx create --name testbuilder
```
```
docker buildx use testbuilder
```
```
docker buildx build --platform linux/amd64,linux/arm64,linux/arm/v7 -t username/imagename --push .
```
