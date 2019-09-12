#Hands On
## Dockerfiles and Building Containers
`FROM rhel:latest

RUN echo "test" > /tmp/test.txt

#This is a comment!
ADD testfile /etc/testfile

CMD echo Yay!
`

* With these 4 directives we can build just about anything
* Each line creates a new layer 

* [Dockerfile reference](https://docs.docker.com/engine/reference/builder/)

---
`cd examples/build`

`docker build -t rhel-test .`

`docker run rhel-test` 

`docker run -it rhel-test /bin/bash`

* You can override the command with something else 
* *Note*: unless you override the filename in the build command, docker is looking for a file named `Dockerfile` 

[Next](ports.md)
