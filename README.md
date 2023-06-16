# CONTAINERS
https://www.youtube.com/watch?v=eGz9DS-aIeY

# DOCKER CONTAINERS 

## INSTALL KALI LINUX
https://www.kali.org/docs/containers/installing-docker-on-kali/
kali@kali:~$ sudo apt update
kali@kali:~$ sudo apt install -y docker.io
kali@kali:~$ sudo systemctl enable docker --now
kali@kali:~$ docker

kali@kali:~$ sudo usermod -aG docker $USER
kali@kali:~$

kali@kali:~$ printf '%s\n' "deb https://download.docker.com/linux/debian bullseye stable" |
sudo tee /etc/apt/sources.list.d/docker-ce.list
  
kali@kali:~$ curl -fsSL https://download.docker.com/linux/debian/gpg |
sudo gpg --dearmor -o /etc/apt/trusted.gpg.d/docker-ce-archive-keyring.gpg
  
kali@kali:~$ sudo apt update
kali@kali:~$ sudo apt install -y docker-ce docker-ce-cli containerd.io

## START DOCKER CONTAINER
start docker
sudo systemctl start docker

auto satrt on boot
$ sudo systemctl enable Docker

verify install
$ sudo docker run hello-world

## CENTOS DEPLOYMENT ON DOCKER CONTAINER
docker pull centos
docker run -d -t --name test centos
docker run -d -t --name test centos
docker exec -it test bash





