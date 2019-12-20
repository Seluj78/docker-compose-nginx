# Self-Signed

[![Docker Cloud Build Status](https://img.shields.io/docker/cloud/build/nickolashkraus/self-signed?color=blue)](https://cloud.docker.com/u/nickolashkraus/repository/docker/nickolashkraus/self-signed)
[![MicroBadger Layers](https://images.microbadger.com/badges/image/nickolashkraus/self-signed.svg)](https://microbadger.com/images/nickolashkraus/self-signed)
[![MicroBadger Version](https://images.microbadger.com/badges/version/nickolashkraus/self-signed.svg)](https://microbadger.com/images/nickolashkraus/self-signed)
[![Releases](https://img.shields.io/github/v/release/NickolasHKraus/self-signed?color=blue)](https://github.com/NickolasHKraus/self-signed/releases)
[![MIT License](https://img.shields.io/github/license/NickolasHKraus/self-signed?color=blue)](https://github.com/NickolasHKraus/self-signed/blob/master/LICENSE)

[Docker Hub](https://cloud.docker.com/u/nickolashkraus/repository/docker/nickolashkraus/self-signed)

Self-Signed provides a working example of how to create a self-signed certificate for NGINX.

https://nickolaskraus.org/articles/how-to-create-a-self-signed-certificate-for-nginx-on-macos/

## Getting Started

To get started with Self-Signed, simply pull the Docker image:

```bash
docker pull nickolashkraus/self-signed
```

Run `self-signed.sh`:

```bash
./self-signed.sh
```

Run NGINX:

```bash
sudo nginx -c $(pwd)/nginx/nginx.conf
```

Run the Docker image:

```bash
docker run \
  -p 1313:1313 \
  nickolashkraus/self-signed:latest
```
