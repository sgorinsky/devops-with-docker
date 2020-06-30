FROM ubuntu:latest

RUN apt-get update -y && apt-get install curl -y 
RUN curl -sL https://deb.nodesource.com/setup_10.x | bash
RUN apt-get install -y nodejs

COPY . .r
RUN ls && cd frontend-example-docker
RUN npm install && npm i -g serve

EXPOSE 80

CMD ["node", "start"]

