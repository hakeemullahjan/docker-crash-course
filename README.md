# docker-crash-course

* #docker build -t node-app .
* #docker run myapp
* #docker run --name myapp_c1 myapp
* #docker start -i myapp_c1
* #docker stop myapp_c1
* #docker run --name myapp_c2 -p 4000:4000 myapp
* #docker run --name myapp_c2 -p 4000:4000 -d myapp
* 
* #docker images
* #docker ps
* #docker ps -a
* #docker image rm myapp
* #docker image rm myapp -f #force
* #docker container rm myapp_c1
* 
* #docker system prune -a #remove all unused images
* 
* #docker build -t myapp:v1 .
* #udo docker run --name myapp_c -p 4000:4000 myapp:v1
* 
* #sudo docker run --name myapp_c_nodemon -p 4000:4000 --rm myapp:nodemon
* 
* #sudo docker run --name myapp_c_nodemon -p 4000:4000 --rm -v /home/hakeemullah/Desktop/Code-lab/docker-crash-course/api:/app -v /app/node_modules  myapp:nodemon
* 
* #docker-componse up 
* #docker-compose down
* #docker-compose down --rmi all --v #remove all containers and images
* sudo docker build -t hakeemullahjan/myapi .
* docker login 
* docker push hakeemullahjan/myapi
* docker pull thenetninjauk/myapi
* https://hub.docker.com/r/hakeemullahjan/myapi