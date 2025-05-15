```sh
# pull docker image
docker pull <docker_image>

# list all locally pulled docker images
docker images

# create and run docker image
docker run <image_repository_name:tag>
docker run <image_id>

# list all containers
docker ps -a
docker ps # list only the running containers

# start a container
docker start <container_name>
docker start <container_id>
docker stop <> # stop container
docker attach <> # attach to container (hooks onto the main process output - not interactive for mysql - is interactive for ubuntu)

# other possible tags with docker run:
-d # detached mode
-e # set environment variables - can be required as per image. for example, mysql image requires MYSQL_ROOT_PASSWORD=<password> environment variable
-p{host_pc_port}:{container_port} # port binding (without space)
--name <name_for_container> # name the container
# image_id/name is always at the end

# delete containers/images
docker rm <container_id>
docker rm <container_name>
docker rmi <image_id>
docker rmi <repository_name:tag>

# docker logs
docker logs <container_id>

# execute a command
docker exec -it <container_id> /bin/bash
# this is executing (exec) the command /bin/bash, interactively (i.e., input/output allowed) (-it) on the container <container_id>
docker exec -it mysql_new mysql -u root -p
# on the docker container "mysql_new" its executing the command interactively "mysql -u root -p" -> login to the running mysql server with username root and password (enter right after this)
```

