The second assignment has been divided into 3 sections:
1 - Docker	(1, 2)
2 - JDBC	(3, 4)
3 - WebApp	(5, 6)

*************************************************************
# 1

Win: download "Docker Toolbox" from docker.org and install it
Other: follow instruction on docs.docker.org

(commands specs on bottom of paragraph)

* CREATE IMAGE:
$ docker build -t IMAGE_NAME PATH/TO/FOLDER/Dockerfile

# or use:

$ cd PATH/TO/MY/Dockerfile
$ docker build -t IMAGE_NAME .

Hint: https://docs.docker.com/engine/tutorials/dockervolumes/#mount-a-host-directory-as-a-data-volume

* CREATE VOLUME:
$ docker volume create VOLUME_NAME
$ docker volume inspect VOLUME_NAME

take PATH and use the following:

* RUN CONTAINER (win)
# docker run -v //DRIVE_LETTER/PATH:/<container path> -p 5432:5432 IMAGE_NAME

Hint: Docker will give to each container a random name, check
it under "docker container list --all" under NAMES or use ID

# TO LOG ALL

Open another console
$ docker logs -f CONTAINER_NAME

Remember to use this command each time CONTAINER_NAME is launched

# INTERACT WITH INTERNAL CONSOLE (INSIDE CONTAINER)
docker exec -it CONTAINER_NAME

*************************************************************
# 2


*************************************************************
# 3
