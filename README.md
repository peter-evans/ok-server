# ok-server
[![](https://images.microbadger.com/badges/image/peterevans/ok-server.svg)](https://microbadger.com/images/peterevans/ok-server)

Docker image for a simple server that responds to any request with "OK"

This image was created for use as a [Kubernetes](https://kubernetes.io/) cluster health check.

## Supported tags and respective `Dockerfile` links

- [`1.0.1`, `1.0`, `latest`  (*1.0/Dockerfile*)](https://github.com/peter-evans/ok-server/tree/master/1.0)

## Usage
Run:
```bash
docker run -d -p 8080:8080 --name ok-server peterevans/ok-server:latest
```
Test:
```
curl http://localhost:8080/my-request/
```

## Reference

[nginx-slim](https://github.com/kubernetes/ingress/tree/master/images/nginx-slim)