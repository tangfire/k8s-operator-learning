FROM golang:1.24.0 as Builder

WORKDIR /app

COPY . .

RUN CGO_ENABLED=0 go build -o ingress-manager main.go

FROM alpine:3.21

WORKDIR /app

COPY --from=builder /app/ingress-manager .

CMD ["./ingress-manager"]