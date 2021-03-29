FROM node:buster

EXPOSE 5000

WORKDIR /usr/src/app

COPY . /usr/src/app

RUN apt-get update && apt-get upgrade -y

RUN node -v && npm -v 

RUN npm install

RUN npm run build

RUN npm install -g serve

CMD ["serve", "-s", "-l", "5000", "build"]
