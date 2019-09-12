# Hands On
## Port Binding 
`docker pull platform-dev-/base/nginx:1.15.7-nginx-nobranch.4`
`docker tag platform-dev-/base/nginx:1.15.7-nginx-nobranch.4 nginx`

--- 

`docker run -d -p 8080:80 -n nginx nginx `

`curl localhost:8080`

* `-d` runs the container in the background. 
* The `EXPOSE` directive in a Dockerfile will bind the port to a high numbered non-standard port. 


[Next](imagemgmt.md)
