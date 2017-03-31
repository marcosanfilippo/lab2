The second assignment has been divided into 3 sections:
1 - Docker	(1, 2, 3)
2 - JDBC	(4)
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

* CREATE VOLUME:
$ docker volume create VOLUME_NAME #skip if you use Dockerfile

Hint: https://docs.docker.com/engine/tutorials/dockervolumes/#mount-a-host-directory-as-a-data-volume

* RUN CONTAINER
# docker run -v //c/<path>:/<container path> IMAGE_NAME

$ docker run -v //d/Mega/POLITO/Applicazioni\ Internet/LAB/lab2/dbdata:/datadb

Hint: Docker will give to each container a random name, check
it under "docker container list --all" under NAMES or use ID
*************************************************************
# 2


*************************************************************
# 3

