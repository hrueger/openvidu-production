# OpenVidu in Docker with custom SSL certificate

[![Available on Docker Hub](https://img.shields.io/badge/available_on-Docker_Hub-blue?logo=docker)](https://hub.docker.com/repository/docker/hrueger/openvidu)

This is a simple Docker Container for the OpenVidu Server and the Kurento Media Server.
It is directly taken from [here](https://github.com/OpenVidu/openvidu/tree/master/openvidu-server/docker/openvidu-server-kms) with the change that it uses the keystore located in `/opt/openvidu/keystore.jks`. The `KEYSTORE_ALIAS` and `KEYSTORE_PW` environment variables have to be present.

## Build
To build a new version, download the latest `openvidu-server.jar` from their [GitHub releases](https://github.com/OpenVidu/openvidu/releases), rename it to `openvidu-server.jar` and copy it into this folder replacing the old one. Then build the image with `docker build .` and use it!