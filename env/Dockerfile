FROM golang:1.7

RUN \
  go get github.com/ethereum/go-ethereum/cmd/geth && \
  rm -rf /go/pkg /go/src && \
  mkdir /blockchain

VOLUME /blockchain

EXPOSE 30303
EXPOSE 8545

ENTRYPOINT ["/go/bin/geth", "--datadir=/blockchain"]
