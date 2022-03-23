# nncase


## Build from source

$ docker buildx build . --tag=nncase:latest --platform linux/amd64 -f Dockerfile.source
$ docker run --it --rm --platform linux/amd64 nncase:latest

## Build from package

$ docker buildx build . --tag=nncase:1.4.0 --platform linux/amd64 -f Dockerfile.1.4.0

