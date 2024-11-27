This repository contains Dockerfile , requirements.txt and app.py file needed to launch a python container in AWS EC2 instnace .

#To build Dockerfile :

docker build -t pythonimg .

#To check whether image is created using Dockerfile :

docker images

#To launch a container using image of this Dockerfile :

docker run -d -p80:5000 --name pythoncontainer pythonimg

#Here the port 80 is port of EC2 instance whereas port 5000 is port of python container

#To check whether container is created using image :

docker ps

