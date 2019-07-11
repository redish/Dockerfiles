FROM golang:1.12.7-alpine3.9

RUN apk update
RUN apk add --no-cache git gcc

RUN go get github.com/pressly/goose
RUN go build -tags='no_postgres no_sqlite3' -i -o ${GOPATH}/bin/goose ${GOPATH}/src/github.com/pressly/goose/cmd/goose
RUN goose --version