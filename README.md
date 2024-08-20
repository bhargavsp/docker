# Docker

## Why we need Docker
If we want to run the different servicess to build an end to end application stack we need a different `libraries and the Dependencies` and each time we change the version of the services by upgrades, we need to check the OS compartibility, to overcome this scenarios we have introduced Docker as it is a container based architecture in which each container have its own lib and dep by itself<br/>
![image](https://github.com/user-attachments/assets/c10fb5c0-1ac1-482b-9640-d2592f19b4b4)

## what are containers
Docker uses the LXC containers for the container service

## containers vs Virtual Machine
![image](https://github.com/user-attachments/assets/9916b7cc-c00d-4fd2-a354-b461e5fcac02)

## Commands
|commands|overview|
|:---:|:---:|
docker run ansible | runs the instance of an ansible application on the docker host if it exists in the docker host else it pulls the image from docker hub and runs the container 
docker run ansible | It runs the conatienr in `Foreground or the attached mode` in which the container's standard input, output, and error streams in real time, we cant use that partiocualr terminal for the executing the other commands as it is in attached mode
docker run -d ansible | runs the container in the detach mode
docker run -it centos bash | Docker runs and logins into the bash container automatically 
docker attach container-id(first 5 letters) | to go back to the running docker conatiner in the detach mode
docker ps | used to see the running containers
docker ps -a | used to see all the running and the stopped containers
docker stop container-name | to stop/forcer-kill the running container
docker rm container-name | to remove the docker container for good
docker images | see available images already in our docker host
docker rmi ansible | to remove the ansible image from our docker host
docker pull ansible | only pulls the ansible image from the docker hub and stores on to the docker host
cat /etc/*release* | to confirm or check the version of the ubuntu we are using EX: Bionic
docker version | check the version of the docker
docker run ubuntu sleep 5 | runs to sleep service in the created ubuntu container and then goes to exited state
docker exec container-name cat /etc/hosts | exec is the execute command used to execute a particular (in this case cat command) command on the created container



## NOTE:
1. If the image inside a container is not running any service or process it goes to an exited state (EX: ubuntu is an OS, not a service to run)
## Docker Editions
1. Community Edition
2. Enterprise Edition


