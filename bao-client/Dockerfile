FROM ubuntu/nginx

RUN  apt-get update && apt-get install 

RUN apt-get install curl -y

RUN apt-get install wget -y

WORKDIR /usr

RUN mkdir downloads && cd downloads

WORKDIR /usr/local

RUN wget https://go.dev/dl/go1.25.5.linux-amd64.tar.gz 

RUN rm -rf /usr/local/go

RUN tar -xvzf go1.25.5.linux-amd64.tar.gz 

RUN  printf "\n export PATH=/usr/local/go/bin" >> /etc/profile

RUN  printf "\n export PATH=/usr/local/go/bin" >> $HOME/.profile



