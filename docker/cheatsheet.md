## install docker and docker-compose
yay -S docker docker-compose  
sudo systemctl start docker.service

## clone your repo
git clone https://link/to/your/repo.git

## add the .env files

## Build and run the containers
sudo docker-compose up -d --build

## Put down docker containers
sudo docker-compose down

## Put down docker containers and delete all volumes
sudo docker-compose down --rmi all --volumes

## To verify what containers are up and what are not
sudo docker ps

## Check logs of a service
sudo docker log <name_of_service(get_from_docker_ps)>

## Check if port is listening
sudo ss -tulpn | grep -E '4040'  
sudo ss -tulpn | grep -E '3000|4040'
