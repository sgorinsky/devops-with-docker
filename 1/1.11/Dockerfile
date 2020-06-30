FROM ubuntu:latest

RUN apt-get update -y && apt-get install curl -y && curl -sL https://deb.nodesource.com/setup_10.x | bash && apt-get install -y nodejs
EXPOSE 8000

COPY . .
RUN cd backend-example-docker && npm i
CMD cd backend-example-docker && npm start
