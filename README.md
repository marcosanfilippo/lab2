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
# Dockerfile must not be specified, it will be searched automatically

docker build -t IMAGE_NAME PATH/TO/Dockerfile

# or use:

cd PATH/TO/MY/Dockerfile
docker build -t IMAGE_NAME .

# Marco's PC: docker build -t lab2 .

Hint: https://docs.docker.com/engine/tutorials/dockervolumes/#mount-a-host-directory-as-a-data-volume

* CREATE VOLUME:
docker volume create VOLUME_NAME
docker volume inspect VOLUME_NAME

take PATH and use the following:

* RUN CONTAINER (win)
# docker run -v //DRIVE_LETTER/PATH_TO_VOLUME:/CONTAINER_PATH_TO_VOLUME -p 5432:5432 IMAGE_NAME

# Marco's PC:
# docker run -v /mnt/sda1/var/lib/docker/volumes/datadb/_data:/datadb -p 5432:5432 lab2

*container path* is /datadb ONLY FOR THIS ASSIGNMENT

Hint: Docker will give to each container a random name, check
it under "docker container list --all" under NAMES or use ID

# TO LOG ALL

Open another console
docker logs -f CONTAINER_NAME

Remember to use this command each time CONTAINER_NAME is launched

# INTERACT WITH INTERNAL CONSOLE (INSIDE CONTAINER)
docker exec -it CONTAINER_NAME bash



*************************************************************
# 2

search for POSTGRES JDBC URL and use it inside java
*************************************************************
# 3
