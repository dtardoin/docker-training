# Hands On
## Images 

`docker images`
---
`docker pull platform-dev/base/rhel:7.7.20190830-d85ca3b8-b1`

* Tags are meant for humans - Image IDs are the authoritative image identifier. 
* Latest is the default tag. 
* Images are comprised of layers 
  * Layers are somewhat similar to Git commits
  * layers are utilized in a caching manner to make rebuilding faster
* How did pulling the Red Hat image look different than busybox?
---
`docker tag platform-dev/base/rhel:7.7.20190830-d85ca3b8-b1 rhel:latest`

`docker images`

[Next](dockerfile.md)
