# docker-cmd


ref-
engine api - https://docs.docker.com/engine/api/v1.24/


Docker commands

docker info
service docker status
service docker start
docker version
docker image ls or docker images

uname -a

docker container ls
docker container ls –a
docker container ps
docker container ps -a
docker container rm CONTAINERID CONTAINERID  ==> multiple delete
docker container rm $( docker container ls –aq)  ==> store in list and delete
docker container stop CONTAINERID 
docker container kill CONTAINERID 
docker container prune -f
docekr container start CONTAINERID 
docker run –d nginx   (d detached) 
docker container run –it nginx /bin/bash
docker container inspect CONTAINERID ==> find ip address
docker container exec –it CONTAINERID /bin/bash  ==> install software
ctrl p q ==> exit from container background running
docker container run ubuntu sleep 30
docker container run ubuntu cat /etc/os-release


port mapping
docker container logs CONTAINERID 
docker container run –d –p 300:80 nginx
netstat –nltp
docker container rename CONTAINERID NEWNAME
docker container restart CONTAINERID
docker container attach CONTANERID
docker container port “container-name”


docker create
docker container create ubuntu
watch docker container diff CONTAINERID

export
docker container export CONTAINERID –o abc.tar
docker image import abc.tar containerImage
docker image save imagename > iamage.tar
docker image load < image.tar


push to docker hub
login to docker hub
docker login
docker images tag ubuntu  hub.docker.com/accountname/imagename/
docker push imagename 





