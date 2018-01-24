# HOW-TO

1. `git checkout https://github.com/sfransonstg/microservicesdocker.git`
1. `mvn clean package`
1. `docker-compose build`
1. `docker swarm init`
1. `docker stack deploy -c docker-compose.yml microservicesdocker`
1. `docker network create -d overlay hello-network`
1. `docker service logs -f microservicesdocker_hello-responder`
1. `docker service scale microservicesdocker_hello-responder=3`
1. `docker service ls`
1. `docker stack ls`
1. `docker stack rm microservicesdocker`


