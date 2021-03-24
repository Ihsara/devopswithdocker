# Start from the alpine image that is smaller but no fancy tools
FROM ubuntu:18.04

#Use /usr/src/app as our workdir. The following instructions will be executed in this location.
WORKDIR /usr/src/app

COPY get-website.sh .

RUN apt-get update; apt-get install -y curl;

#When running docker run the command will be ./hello.sh
CMD ./get-website.sh
