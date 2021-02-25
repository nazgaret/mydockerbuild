FROM golang:1.15

CMD go 

WORKDIR /server

RUN apt-get update && apt-get install -y --no-install-recommends

COPY server.go .

COPY go.mod .

EXPOSE 1111

RUN go build server.go

CMD ./server


