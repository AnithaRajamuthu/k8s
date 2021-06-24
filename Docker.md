# Docker 

## Introduction

Tool used to automate the deployment of applications in light weight containers so that applications can 
work efficiently in different environment


## Setting up Docker

Editions – Community , Enterprise
 ``` 
  Installation :https://www.docker.com/products/docker-desktop
  
 ```
    Docker hub   : https://hub.docker.com/

![image](https://user-images.githubusercontent.com/34361796/123225650-8abfd780-d4f0-11eb-9047-2343e5869494.png)

![image](https://user-images.githubusercontent.com/34361796/123225828-b9d64900-d4f0-11eb-950d-afc42a44b356.png)

Docker Vs VM

![image](https://user-images.githubusercontent.com/34361796/123225883-c5c20b00-d4f0-11eb-94e2-332e411542a3.png)


## Docker Commands
  ```
$docker run nginx
$docker pull nginx
$docker ps
$docker ps -a

$docker run ubuntu
$docker run ubuntu sleep 5
$docker ps -a 
$docker exec <image name> cat etc/hosts
$docker run -d ubuntu
$docker attach <containerid>

$docker run centos
$docker run -it centos bash
   $cat /etc/release
$docker ps 
$docker run -d centos sleep 20
$docker rm <images>
$docker exec 
$docker version

$docker run helloworld
$docker run –p 80:5000 helloworld

$docker run mysql
$docker stop mysql
$dcker rm mysql

$docker run jenkins
$docker run -p 8080:8080 jenkins

Run container using redis image

$docker run redis
$docker run redis:4.0 -- tag

Default container port : 5000
  ```
## Port mapping and volume mapping

  ```
$docker run -p 80:5000 <app name>

$ docker run -p 8306:3306 mysql
$docker run -p 3306:3306 mysql
$docker run -v  /opt/datadir:/var/lib/mysql mysql
$docker logs <imagename>
  ```

## Images

  ```
$docker build .
  ```
  
