FROM golang:1.15

CMD go 

WORKDIR /hello

RUN apt-get update && apt-get install -y --no-install-recommends

COPY hello.go .

COPY go.mod .

RUN go build hello.go

CMD ./hello


