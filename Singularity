BootStrap: docker
From: ubuntu:latest

%post
    apt-get update
    apt-get -y install python3-pip
    pip3 install asciinema

%runscript
exec asciinema "$@"
