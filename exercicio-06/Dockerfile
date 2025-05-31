FROM golang:1.19 AS builder

WORKDIR /app

COPY main.go .

RUN go build -o gs-ping main.go

FROM alpine

COPY --from=builder /app/gs-ping /gs-ping

CMD ["/gs-ping"]
