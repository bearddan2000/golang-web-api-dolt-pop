FROM ubuntu:latest

COPY bin/ ./

ARG DEBIAN_FRONTEND=noninteractive

RUN apt-get update \
    && apt-get install -y --no-install-recommends \
      apt-transport-https \
      software-properties-common \
      golang-go \
    && chmod +x ./main.go \
    && chmod +x ./dependcy.sh
# Add docker-compose-wait tool -------------------
ENV WAIT_VERSION 2.7.2

ADD https://github.com/ufoscout/docker-compose-wait/releases/download/$WAIT_VERSION/wait /wait

RUN chmod +x /wait

CMD ["./dependcy.sh"]
