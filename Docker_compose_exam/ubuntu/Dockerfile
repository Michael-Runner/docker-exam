FROM ubuntu:22.04
RUN echo 'APT::Install-Suggests "0";' >> /etc/apt/apt.conf.d/00-docker
RUN echo 'APT::Install-Recommends "0";' >> /etc/apt/apt.conf.d/00-docker

RUN echo uname -a  >> /etc/satrt.log
RUN echo df -h  >> /etc/satrt.log

RUN apt update
RUN apt upgrade
RUN apt install -y neofetch
RUN neofetch >> neo.log

RUN useradd -ms /bin/bash apprunner
USER apprunner