# Dockerized PXE server

> based on [https://github.com/ferrarimarco/docker-pxe](https://github.com/ferrarimarco/docker-pxe)

### Pre-requirements
If you do not have Docker installed:
```bash
$ curl -fsSL get.docker.com -o get-docker.sh && sh get-docker.sh
```

## How to run
1. Clone repository and open it
2. Run ```docker build -t pxe .```
3. Then ```docker run -it --rm --net=host pxe --dhcp-range=x.x.x.x,y.y.y.y```
P.S. In the third point instead of x.x.x.x,y.y.y.y you need to put range of IP addresses that can be given to the user.
