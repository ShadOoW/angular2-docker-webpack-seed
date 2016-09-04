# Set the base image to Ubuntu
FROM ubuntu:16.04

# Add apt-get config
ADD docker-config/apt.conf /etc/apt/apt.conf

# Install Node.js and other dependencies
RUN apt-get update
RUN apt-get -y install curl git nginx gettext ca-certificates
RUN curl -sL https://deb.nodesource.com/setup_6.x | bash -
RUN apt-get -y install python build-essential nodejs
