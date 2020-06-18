FROM ubuntu:latest

RUN apt-get update
RUN DEBIAN_FRONTEND="noninteractive" apt-get -y install tzdata
RUN apt-get install -y php7.4
RUN apt-get install -y apache2

#VOLUME C:\xampp\htdocs\GitDockerProjekt:/var/www/html
ADD https://github.com/stillerndenacht/GitDockerProjekt/blob/master/indexV.php /var/www/html
WORKDIR /var