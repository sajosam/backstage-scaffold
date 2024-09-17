FROM golang:1.23 AS builder
WORKDIR /backend

COPY . .

RUN go get
RUN CGO_ENABLED=0 GOOS=linux go build -o app

EXPOSE 8080

CMD ["./main"]