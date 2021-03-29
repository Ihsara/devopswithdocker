FROM golang:1.16-buster

EXPOSE 8080

WORKDIR /usr/src/app

COPY . /usr/src/app

RUN apt-get update && apt-get upgrade -y

RUN go build

RUN go test ./...

ENV REQUEST_ORIGIN=*

ENV PORT=8080

CMD = [".", "./server"]

