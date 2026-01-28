# Day 01 – Docker Basics

## Day 01 started with the following 
- What is Docker
- Difference between VM and Container
- Docker architecture
- Installed Docker

## Commands Practiced
```bash
docker --version
docker run hello-world
docker ps 
docker ps -a 
docker rm "conatiner name"
docker rmi "image name"

## issue faced
. while installing docker faced the issue DNS name was not resolving and need to install ifconfig in new ubuntu machine with following CMD.
 network:
    4  sudo netplan apply
    5  sudo nano /etc/netplan/*.yaml
    6  ifconfig
    7  apt install net-tools
    8  apt-get updateexit
    9  sudo nano /etc/netplan/*.yaml
   10  sudo apt update
   11  sudo apt upgrade -y
   12  sudo reboot
##Outcome
. after this able to install docker with following CMD 

sudo apt update
   94  sudo apt install docker-ce docker-ce-cli containerd.io docker-buildx-plugin docker-compose-plugin
   95  sudo systemctl status docker
   96  sudo systemctl start docker
##Result

Docker has been installed
first container "Hello-world" has been pulled and run successfully
