# Java (JRE or JDK version 8, 11 or 17) with Node.js 16 or 18 LTS Dockerfile

[![Docker Automated build](https://img.shields.io/docker/automated/timbru31/java-node.svg)](https://hub.docker.com/r/timbru31/java-node/)
[![buildx Status](https://github.com/timbru31/docker-java-node/workflows/buildx/badge.svg)](https://github.com/timbru31/docker-java-node/actions?query=workflow%3Abuildx)
[![Lint Dockerfiles](https://github.com/timbru31/docker-java-node/workflows/Lint%20Dockerfiles/badge.svg)](https://github.com/timbru31/docker-java-node/actions?query=workflow%3A%22Lint+Dockerfiles%22)

A minimal Dockerfile based on Eclipse Temurin's OpenJDK JRE or JDK 8/11 Dockerfile (regular, alpine) with Node.js 16 LTS (Gallium) or 18 LTS (Hydrogen) installed.

## What's included

- JRE or JDK 8/11/17
- Node.js 16 LTS (Gallium) or 18 LTS (Hydrogen)
- bundled npm that comes with the respective Node.js version (latest for Node.js LTS v16+ on alpine, see [why](https://gitlab.alpinelinux.org/alpine/aports/-/commit/25b10bd1a93e12a7e49fee38b0a229281ae49fb7))
- yarn
- curl

### Available platforms

These Dockerfiles leverage the new `buildx` functionality and offer the following platforms:

- linux/amd64
- linux/arm64 (not for alpine)
- linux/arm/v8 (not for alpine)
- linux/ppc64le (not for alpine)

---

Built by (c) Tim Brust and contributors. Released under the MIT license.
