FROM ubuntu:latest

RUN apt-get update -y && apt-get install curl -y 
RUN curl -sL https://deb.nodesource.com/setup_10.x | bash
RUN apt-get install -y nodejs

COPY . .
RUN cd frontend-example-docker && npm install && npm i -g serve

EXPOSE 80

CMD cd $(ls | grep frontend) && npm start

