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

##### push my_image to my_project in GCR under image name gcr_name
be aware of different storage zones:
- gcr.io - US
- asia.gcr.io - Asia
- eu.gcr.io - EU member states
- us.gcr.io - US
```
docker tag my_image gcr.io/my_project/gcr_name
docker push gcr.io/my_project/gcr_name
```

##### delete all docker images
- a "all"
- q "quiet", return only image ids
```
docker rmi $(docker image ls -aq)
```
