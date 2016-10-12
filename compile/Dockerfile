FROM golang

RUN go get -v github.com/owlab-exp/ipify-api \
    && CGO_ENABLED=0 GOOS=linux go build -v -a -installsuffix nocgo -ldflags="-s -w" -o /ipify-api github.com/owlab-exp/ipify-api
