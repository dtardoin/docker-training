# Background 

## Key Docker Concepts 
* Docker Daemon / CLI  - `docker version`
* Image 
  * Read only 
  * Built by you or pulled out of Artifactory 
  * Very similar to a Jar or a Zip file
  * Done correctly - gives you an audit trail of exactly what's in the container
* Container 
  * Run time of an image 
  * Contains everything needed to run an application
  * Completely isolated from other containers and other things running on host system
* Registry 
  * storage for built images 
  * `docker push` and `docker pull` 
  * Artifactory is the currently supported registry for OCC
  * Dockerhub 


[Next](../hands-on/dockerpull.md)
