# NGINX golden image

The image uses debian:jessie-slim from quay.io as default source which can be overriden via a runtime argument.

## Build
```
docker build -t nginx-base --build-arg DEBIAN_IMAGE=debian-base .
```
If you don't specify --build-arg, then Docker will use the default value in the ARG.