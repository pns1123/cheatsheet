##### run a bash shell in the (running) container mycontainer
- -i (interatively)
- -t (allocate a pseudo TTY)
```
docker exec -it mycontainer /bin/bash
```
