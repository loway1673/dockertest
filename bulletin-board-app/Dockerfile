FROM ubuntu:latest

RUN apt-get update --fix-missing
RUN apt-get -y install nodejs
RUN apt-get -y install npm

WORKDIR /usr/src/app
COPY package.json .
RUN npm install

EXPOSE 8080
CMD [ "npm", "start" ]

COPY . .
