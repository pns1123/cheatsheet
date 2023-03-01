##### run a bash shell in the (running) container mycontainer
- -i (interatively)
- -t (allocate a pseudo TTY)
```
docker exec -it mycontainer /bin/bash
```

##### publish / map a container port
- -p (publish)
- map container port 8069 to host port 8042
```
docker run -p 8042:8069
```
