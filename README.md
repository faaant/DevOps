# DevOps

### [DockerHub repository](https://hub.docker.com/repository/docker/faaant/nodejs-app)

## First step:

Build the image:

```
docker build . -t nodejs-app
```

## Second step:

Check all available images and their ids:

```
docker images
```

## Third step:

Run the container with memory(3GB) and CPU limits(1 core) on `80` port:

```
docker run -m="3g" --cpus="1.0" --rm --name nodejs-app -p 80:80 -d nodejs-app
```