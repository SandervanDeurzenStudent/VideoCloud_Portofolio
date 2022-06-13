**_Clarification:
Design and implement: You design a release process and implement a continuous integration and deployment solution (using e.g. Gitlab CI and Docker).
_**

### 1. docker
Docker allows developers to make lightweight containers of their application that can be run virtually anywhere. I use a Github workflow package called Docker Publish which automaticly creates images on pushes to master. 


 docker container 
 
![DockerContainers](https://user-images.githubusercontent.com/73832880/171404191-8f0ca376-d4eb-4f15-ae36-935fb3d14014.JPG)

Docker images

![DockerImages](https://user-images.githubusercontent.com/73832880/171404264-3d343cc3-ab7a-4165-958b-0b5650dff166.JPG)


My Backend, Frontend and database are running in docker containers. This is configurated by a .yaml file as seen below.

docker-compose.yaml

![compose_yaml](https://user-images.githubusercontent.com/73832880/171404230-74161da8-40a6-402f-b004-d2498c88fdb7.png)



### 2. automatic testing

By making tests you can check if everything works as it's supposed to, Therefore it might be a good idea to run those test everytime you make a change, as in a push. The code below ensures that with every push to the master branch, every test gets run.

maven.yaml

![mavenyaml](https://user-images.githubusercontent.com/73832880/171806833-17507762-d140-4ed3-8b02-90f4510ac7fd.JPG)


Github Workflows for CI and CD

![workflows_github](https://user-images.githubusercontent.com/73832880/171806983-fa7448de-9d35-4321-9a88-787f267ba9ac.JPG)
