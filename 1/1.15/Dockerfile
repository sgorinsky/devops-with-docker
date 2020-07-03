FROM ubuntu:16.04

RUN apt-get update && apt-get install curl -y
COPY start.sh .
RUN chmod +x start.sh

ENTRYPOINT ["./start.sh"]
