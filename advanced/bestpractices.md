# Advanced
## Best Practices

### Dockerfile directive order 
* The ordering of your directives will impact build time based on caching. 
  * example: install dependencies before adding code.

### Do one thing 
* A single container should only do one thing (not necessarily run one process)
* If you need an init system (supervisord, systemd), you would probably benefit more from multiple containers 

### Don't use Root
Just because it's a container, you still shouldn't be using root as the user running your service.  It's still a security issue for the same reason you wouldn't do that on a VM. 


### Build the smallest image possible
Don't install packages you won't need runtime, and try to optimize for the smallest image possible.  The smaller the image is, the quicker it is to build, pull and push across the network. 


