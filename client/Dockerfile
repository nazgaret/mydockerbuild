FROM golang:1.15

CMD go 

WORKDIR /client

RUN apt-get update && apt-get install -y --no-install-recommends

COPY client.go .

COPY go.mod .

RUN go build client.go

CMD ./client

