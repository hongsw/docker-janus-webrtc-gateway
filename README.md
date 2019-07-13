# About

-   This image contains the meetecho janus webrtc gateway  ([https://github.com/meetecho/janus-gateway](https://github.com/meetecho/janus-gateway))

-   It uses the google stun server

-   This repository is published here: [https://hub.docker.com/r/efacilitation/docker-janus-webrtc-gateway/
](https://hub.docker.com/r/efacilitation/docker-janus-webrtc-gateway/)

## Limitations

Disables RabbitMQ and MQTT

## Build

`docker build -t efacilitation/docker-janus-webrtc-gateway .`

## Ports

| Port   | Description        |
|--------|--------------------|
| 80     | HTML-Examples      |
| 443    | HTML-Examples(SSL) |
| 8088   | RESTful API        |
| 8188   | WebSocket API      |

## Environment variables

No environment variables are needed for this image.

## Linked Containers

This container does not need any container linked to.

## Run

'sudo docker run -d -p 80:80 -p 443:443 -p 7889:7889 -p 7088:7088 -p 8088:8088 -p 8188:8188 hongsw/docker-janus-webrtc-gateway:latest
