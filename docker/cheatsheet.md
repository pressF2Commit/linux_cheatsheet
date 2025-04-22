## install docker and docker-compose
```bash
yay -S docker docker-compose  
sudo systemctl start docker.service
```

## clone your repo
```bash
git clone <url/to/your/repo.git>
```
## add the .env files

## Build and run the containers
```bash
sudo docker-compose up -d --build
```

## Put down docker containers
```bash
sudo docker-compose down
```

## Put down docker containers and delete all volumes
```bash
sudo docker-compose down --rmi all --volumes
```

## To verify what containers are up and what are not
```bash
sudo docker ps
```

## Check logs of a service
```bash
sudo docker log <name_of_service>
# get name of service from <docker ps>
```

## Check if port is listening
```bash
sudo ss -tulpn | grep -E '4040'  
sudo ss -tulpn | grep -E '3000|4040'
```