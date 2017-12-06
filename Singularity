BootStrap: docker
From: ubuntu:latest

%post
    export http_proxy=http://webproxy.metoffice.gov.uk:8080
    apt-get update
    apt-get -y install python3-pip locales
    pip3 install asciinema
    locale-gen en_GB.UTF-8


%environment
    LANG=en_GB.UTF-8
    LANGUAGE=en_GB:en
    LC_ALL=en_GB.UTF-8
    export LANG LANGUAGE LC_ALL
    http_proxy=http://webproxy.metoffice.gov.uk:8080

%runscript
exec asciinema "$@"
