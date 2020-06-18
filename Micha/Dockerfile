FROM ubuntu:latest

 

RUN apt-get update 

RUN DEBIAN_FRONTEND="noninteractive" apt-get -y install tzdata

RUN apt-get install -y php5.6

RUN apt-get install -y  apache2
VOLUME ~/php-verzeichnis:/var/www/html
 

WORKDIR /var
