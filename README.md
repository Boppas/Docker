# Docker
Dockerfiles
Dockerfile is a declarative way of creating our own images. Docker will give us some syntax to create our own images.

File name should Dockerfile. docker command should run where your Dockerfile exists.

How to build image from Dockerfile

docker build -t [docker-hub-URL]/[your-username]/[image-name]:version .

How to push image to Dockerhub

docker push [docker-hub-URL]/[your-username]/[image-name]:version

to filter images by label
docker images --filter "label=[whatconditiontosearch]=[whatitsmappedto]

docker run env:v1 ping -c 4 google.com / This command prints goole.com 4 times inside the container env:v1

docker ps -a /this command gives the logs of a particular container

docker network create [name-for-the-network] / will create a bridge network with the name given

docker containers are ephemeral(Temporary). When you remove a container by default it will delete the data

Kinds of network on Docker
1.Bridge - bydefault
2.Host
3.Overlay
4.macvlan

Default bridge network can not resolve on names, Docker recommends to create our own bridge network
When we create our own bridge network containers are isolated from other projects and we can communicate using names between Containers.
