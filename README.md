# Dockerized PXE server

> based on [https://github.com/ferrarimarco/docker-pxe](https://github.com/ferrarimarco/docker-pxe)

### Pre-requirements
Docker!
```bash
$ curl -fsSL get.docker.com -o get-docker.sh && sh get-docker.sh
```

## How to run
1. Clone repository and open it
2. Run ```docker build -t pxe .```
3. Then ```docker run -it --rm --net=host pxe --dhcp-range=x.x.x.x,y.y.y.y```
