FROM golang:1.19-alpine AS builder
WORKDIR /

COPY go.mod hello.go ./
RUN go build

FROM scratch
COPY --from=builder hello /
CMD [ "/hello" ]