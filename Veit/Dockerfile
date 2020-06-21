FROM ubuntu:latest

RUN apt-get update
RUN DEBIAN_FRONTEND="noninteractive" apt-get -y install tzdata
RUN apt-get install -y php7.4
RUN apt-get install -y apache2
RUN apt-get install git

RUN apache2ctl start
#VOLUME /c/xampp/htdocs/GitDockerProjekt:/var/www/html
#ADD https://github.com/stillerndenacht/GitDockerProjekt/blob/master/index_v.php /var/www/html
RUN cd /var/www/ \ 
mkdir gitphp \ 
cd gitphp \
git clone https://github.com/stillerndenacht/GitDockerProjekt.git .

#CMD ["systemctl", "start apache2"]
#CMD ["cd /var/www/gitphp", "git pull origin master"]
#CMD ["cd", ""]
WORKDIR /var