FROM debian

RUN apt-get update && apt-get upgrade -y && apt-get install wget bzip2 -y
RUN wget http://dl.4players.de/ts/releases/3.5.0/teamspeak3-server_linux_amd64-3.5.0.tar.bz2
RUN tar xjf teamspeak3-server_linux_amd64-3.5.0.tar.bz2 && rm teamspeak3-server_linux_amd64-3.5.0.tar.bz2

WORKDIR /teamspeak3-server_linux_amd64
RUN touch .ts3server_license_accepted

CMD [ "./ts3server_minimal_runscript.sh" ]
#-p 9987:9987/udp -p 10011:10011 -p 30033:30033
