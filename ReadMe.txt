26th June 2020
==============

After successful login into a brand new DO droplet.. run the following 

apt-get update
apt-get upgrade 


curl -fsSL get.docker.com -o get-docker.sh
sudo sh get-docker.sh

sudo curl -L "https://github.com/docker/compose/releases/download/1.23.1/docker-compose-$(uname -s)-$(uname -m)" -o /usr/local/bin/docker-compose
sudo chmod +x /usr/local/bin/docker-compose

docker -v 
docker-compose -v

$ docker-compose -f docker-compose.prod.yml build
$ docker-compose -f docker-compose.prod.yml up -d
$ docker exec -d btreProd_container python3 manage.py runserver 0.0.0.0:8000

$ cd ~/btre_23rdfeb/app
$chmod +x entrypoint.prod.sh

23rd Feb 2020
=============
$ docker-compose -f docker-compose.prod.yml build
$ docker-compose -f docker-compose.prod.yml up -d
$ docker exec -d btreProd_container python3 manage.py runserver 0.0.0.0:8000

At web-browser: localhost

16th Feb 2020
=============
$ docker-compose -f docker-compose.prod.yml build
$ docker-compose -f docker-compose.prod.yml up -d
$ docker exec -it btreProd_container bash
$ python3 runserver 0.0.0.0:8000

At web-browser: localhost:1337
