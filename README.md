# docker
Installing Docker
sudo apt-get remove docker docker-engine docker.io
sudo apt-get update
sudo apt-get install \ apt-transport-https \ ca-certificates \ curl \ gnupg-agent \ software-properties-common
curl -fsSL https://download.docker.com/linux/ubuntu/gpg | sudo apt-key add -
sudo apt-key fingerprint 0EBFCD88
sudo add-apt-repository \ "deb [arch=amd64] https://download.docker.com/linux/ubuntu \ $(lsb_release -cs) \ stable"
sudo apt-get update
sudo apt-get install docker-ce docker-ce-cli containerd.io

sudo docker run hello-world
List Docker CLI commands
docker
docker container --help
Display Docker version and info
docker --version
docker version
docker info
Execute Docker image
 docker run hello-world
list Docker images
docker image ls
List Docker containers (running, all, all in quiet mode)
docker container ls
docker container ls --all
docker container ls -aq
Remove docker image
docker rmi <<imageName>>
