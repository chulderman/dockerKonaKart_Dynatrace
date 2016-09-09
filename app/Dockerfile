FROM debian:jessie
MAINTAINER Chase Hulderman <chase@hulderman.com>

#Update the repository
RUN apt-get update

#Install Java Runtime Environment for KonaKart
RUN apt-get install -y openjdk-7-jre

#Add files to directories on Docker Container
CMD echo "Adding installation script"
ADD ./installation.sh /opt/
ADD ./konakart-installation /tmp/

#Instrument with Dynatrace Agent
ADD ./dynatrace-agent-6.3.0.1305-unix.jar /opt/
ADD ./startkonakart.sh /opt/

#Listen on default konakart port
EXPOSE 8780

#Run konakart
CMD /bin/bash /opt/installation.sh

#Example usage:
# sudo docker run -d -p 8080:8780 --name konakart_app -e DB_ADDRESS=x.x.x.x -e DB_PORT=PORT –e repository_name
