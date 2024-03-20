# Docker

## Enter Docker VM on Mac OS

```shell
docker run -it --rm --privileged --pid=host alpine:edge nsenter -t 1 -m -u -n -i sh
```

`--privileged` Extended privileges to this container https://docs.docker.com/engine/reference/run/#runtime-privilege-and-linux-capabilities
`--pid=host` Run in the host PID namespace https://docs.docker.com/engine/release-notes/prior-releases/#runtime-25
`nsenter` Namespace Enter https://man7.org/linux/man-pages/man1/nsenter.1.html
`-t 1` Target PID to get contexts from
`-m` Enter the mount namespace
`-u` Enter the UTS namespace
`-n` Enter the network namespace
`-i` Enter the IPC namespace
