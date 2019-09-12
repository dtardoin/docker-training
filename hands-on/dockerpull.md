# Hands On
## Registries and Docker Pull 

* Registries are artifact storage for Docker Images 
* Workflow: 
  1. CI: build & push to registry 
  1. Server: pull and run 
* OCC's registries are hosted in artifactory: 
  * svnserver.theocc.com:8443 (docker-dev-local) 
  * svnserver.theocc.com:8444 (docker-test-local) 
  * svnserver.theocc.com:8445 (docker-prod-local)


Let's pull our first image:  
`docker pull busybox:latest`

And verify that it is in our local image store:  
`docker images`

[Next](dockerrun.md)
