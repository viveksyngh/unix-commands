##  Docker related commands 
*Display kernel version*
```
uname -r
```
*Install Docker*
```
sudo apt-get install docker-engine
```
*Start the docker dameon*
```
sudo service docker start
```
*Verify docker is installed correctly.*
```
sudo docker run hello-world
```
*Downloads docker ubuntu image and run that*
```
sudo docker run -it ubuntu
```
*List all running containers with details*
```
sudo docker ps 
```
*List all containers (running + offline)*
```
sudo docker ps -a
```
*List all latest created containers including offline containers*
```
sudo docker ps -l
```
*Stop a container*
```
sudo docker stop container_name
```
*Removes a container*
```
sudo docker rm {container_id}
```
*Flags during run command*

  *--name : to give name for container*

  *-d : To run the container in detach mode(Background)*

  *-e or --env : To set the enviornment in docker like MYSQL_ROOT_PASSWORD=123*

  *-p : To bind the docker port to host port, like 3306:3306*
```
sudo docker run --name db -d -e MYSQL_ROOT_PASSWORD=123 -p 3306:3306 mysql:latest
```
*Executes command in terminal in inetractive mode on container named db*
```
sudo docker exec -it db /bin/bash
```
*Build a docker image with a doker file with given name and tag*
```
sudo docker build -t {imagename:tag} .
```
*To list all docker images*
```
sudo docker images
```

