# Installing Ansible

Install Ansible on Ubuntu

```
$ sudo apt update
$ sudo apt install software-properties-common
$ sudo add-apt-repository --yes --update ppa:ansible/ansible
$ sudo apt install ansible-base
```

# Installing [AWX](https://github.com/ansible/awx) 19.3.0 in Docker on Ubuntu 20.04

Install Git
```
$ sudo apt install git -y
```

Install pip for python3
```
$ sudo apt install python3-pip
```

Install Docker by following these instructions
https://docs.docker.com/engine/install/ubuntu/#installation-methods

Install Docker Compose Python module (I believe this will install Docker Compose as well)
```
$ pip install docker-compose
```

Add your user to the docker group [source](https://stackoverflow.com/questions/47854463/docker-got-permission-denied-while-trying-to-connect-to-the-docker-daemon-socke)
```
sudo usermod -a -G docker [user]
newgrp docker
```
Logout and login again

Now follow these instructions to install AWX using Docker Compose
https://github.com/ansible/awx/blob/devel/tools/docker-compose/README.md

Easy... Not!

