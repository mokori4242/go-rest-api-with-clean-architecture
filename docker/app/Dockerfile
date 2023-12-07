FROM golang:1.20

WORKDIR /app

RUN apt-get update && apt-get install -y git \
    && go install github.com/cosmtrek/air@latest

EXPOSE 8080
CMD ["air", "-c", ".air.toml"]