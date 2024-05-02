# dockercmd

## Running Containers
```docker ps```

## run container 
```docker run ubuntu```

--> if no image is present then it will download first

## to get access in terminal
```docker run -it ubuntu``` 

## see all the docker images
```docker images```

## to pull the image
```docker pull ubuntu:16.04```

if you dont mention the version it will download the latest one

## to get the running container 
```docker container ls```

you can copy container id and you go into their interactive env using cli via cmd above to get access in teermingal 

## stop the container 
```docker stop 'container id'```

## All the container running
```docker ps -a```

## put direct to terminal of image
```docker run ubuntu echo Hey```
ouput :- Hey

 ===========================================

## port map
```docker run -d -p  8080:80 nginx```

![Alt text](./image.png)
![Alt text](image-1.png)

## docker commit 
```docker commit -m "message added" containerID imageName``` // this command will add 

first copy that container id then 
`docker start id`
then
`docker exec -it id bash`


============================

## to build the image using docker file
```docker build -t MyImage:1.1 .```

# inspect and see which container are on networks
docker network inspect bridge

https://app.eraser.io/workspace/yTPql82lXyOpbyX63Xgn 

# list of dockr network
```docker network ls```

# creqte your own network
```docker network create -d bridge customMyNetwork```

# to inspect network
```docker network inspect customMyNetwork```

# docker volume
 ```docker run -it -v /home/Desktop/test-folder:/home/abc ubuntu```
