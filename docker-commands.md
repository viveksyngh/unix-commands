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
