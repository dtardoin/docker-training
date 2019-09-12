# Advanced
## Other Useful Docker Commands and Flags

### Exec Into a Running Container
Use `docker exec` to run a command in an already running container. 

```
docker run -d -n webserver nginx 
...
docker exec -it webserver /bin/bash 
```

*Note*: This should be more for debugging than actually a part of your workflow.a

### Environment Variables 
Allows you to override settings inside of a container at runtime. 

```
docker run -e TEST_VAR="hello world!" -it rhel /bin/bash

echo $TEST_VAR
```

### Volume Mount
```
docker run -v $(pwd):/tmp -it rhel /bin/bash 

ls /tmp

```


*Note*: if used incorrectly, this can violate 

### Log 

```
docker run -d -p 8080:80 --name=nginx-webserver nginx 

docker logs -f nginx-webserver
```

### CMD vs ENTRYPOINT 
*  [Entrypoint allows you to run container as an executable with parameters](https://goinbigdata.com/docker-run-vs-cmd-vs-entrypoint/)

[Next](orchestrators.md)
