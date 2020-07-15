FROM ubuntu:latest

COPY . .
WORKDIR /backend-example-docker

RUN apt-get update -y && \
    apt-get install curl -y && \
    curl -sL https://deb.nodesource.com/setup_10.x | bash && apt-get install -y nodejs && \
    npm i && \
    apt-get purge -y --auto-remove curl && \ 
    rm -rf /var/lib/apt/lists/*

CMD npm start