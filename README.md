# Docker
# Docker
##Getting Started
- community 
- enterprise - certified image management , image security 
## Docker commands
- docker run nginx < install docker image if not there and run the image in a container>
- docker ps < list all running container with info>
- docker ps -a < see all images that exited>
- docker stop <contid/name>
- docker rm <contname/contid> ->remove container to reclaim disk space
- docker images < list all images and sizes>
- docker rmi imgname -> removes image name , make sure to delete all dependent containers using the image
- docker pull imgname --> just pulls the image and not download
-docker run ubuntu sleep 100 --> run ubuntu conatiner for 100s and then exits
- docker -d run imgname --> run in detach mode
- docker exec <contid> cat /etc/*release* --> execute a image and runs a command on that
- docker stop $(docker ps -aq) --> stop all containers at once
- docker rm $(docker ps -aq) --> remove all containers at once
- docker run -d --name webapp nginx:1.14-alpine <use name webapp and use the specified image>
- docker rmi $(docker images -aq) -- delete all images at once 
