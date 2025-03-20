FROM golang:1.21 AS builder
WORKDIR /app

COPY main.go .

RUN go mod init datetime-app || true
RUN go mod tidy

RUN GOOS=linux GOARCH=amd64 go build -o datetime-app main.go

FROM alpine:latest
WORKDIR /root/

COPY --from=builder /app/datetime-app .

RUN chmod +x datetime-app

CMD ["./datetime-app"]
