FROM golang:1.22-alpine

ENV GIN_MODE release
WORKDIR /home/astarion

COPY data/main .

ENTRYPOINT [ "./main" ]
