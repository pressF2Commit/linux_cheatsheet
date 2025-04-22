# install docker
curl -fsSL https://get.docker.com -o get-docker.sh
sudo sh get-docker.sh

# install docker-compose
sudo curl -L "https://github.com/docker/compose/releases/download/v2.24.0/docker-compose-$(uname -s)-$(uname -m)" -o /usr/local/bin/docker-compose
sudo chmod +x /usr/local/bin/docker-compose

# clone your repo
git clone https://link/to/your/repo.git

# add the .env files

# Build and run the containers
sudo docker-compose up -d --build

# Put down docker containers
sudo docker-compose down

# Put down docker containers and delete all volumes
sudo docker-compose down --rmi all --volumes

# To verify what containers are up and what are not
sudo docker ps

# Check logs of a service
sudo docker log "name of service/get from docker ps"

# Check if port is listening
sudo ss -tulpn | grep -E '4040'
sudo ss -tulpn | grep -E '3000|4040'
