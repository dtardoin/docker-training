# Hands On
## Exercise

#TODO: copy code here, attribute to edgar
Code is contained in this repository in `examples/exercise`

## Write a Dockerfile
* Add a Dockerfile to the top of that directory 
* It should inherit from a java-jdk image from artifactory 
* Download and install Gradle 4.4.1 from artifactory into /apps
* Add code into container in /occ/demo-app
* Have gradle build code 
* Set the command to start the webservice 

## Run the container 
* Run the container and port bind it (the application runs on port 8080)
* Test that the API works using curl. 


[Next](../advanced/compose.md)
