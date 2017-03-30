The second assignment has been divided into 3 sections:
1 - Docker	(1, 2, 3)
2 - JDBC	(4)
3 - WebApp	(5, 6)

*************************************************************
# 1

Win: download "Docker Toolbox" from docker.org and install it

* CREATE IMAGE:
$ docker build -t IMAGE_NAME PATH/TO/FOLDER/Dockerfile

# or use:

$ cd PATH/TO/MY/Dockerfile
$ docker build -t IMAGE_NAME .

* CREATE VOLUME:
$ docker volume create datadb
// create folder datadb ?

* RUN CONTAINER
$ docker run -v /datadb:/lab2volume lab2
*************************************************************
# 2


*************************************************************
# 3

