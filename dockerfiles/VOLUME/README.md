### volume

docker volume create [name-of-the-volume] - creating volume

We can even create a directory and attach to docker container. But we can not list them on docker as its not created using docker and is called anonymus volues

Attach the volume to container

docker run -d -v [name-of-the-volume]:path -p (hostport and the port which is open) 80:80 

Inside host we will have a directory for volume.
This directory can be mounted with any path inside the container
In Nginx its like
/var/lib/docker/volume/nginx_data:/usr/share/nginx/html 
