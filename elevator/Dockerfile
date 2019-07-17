FROM golang:1.10
MAINTAINER "jesse.ha" <jesse.ha@kakaocorp.com>

COPY . /go/src/2019-blind-2nd-elevator/elevator 
WORKDIR /go/src/2019-blind-2nd-elevator/elevator/cmd/elevator

RUN go get ./
RUN go build

RUN mv /go/src/2019-blind-2nd-elevator/elevator/dataset /go/src/2019-blind-2nd-elevator/
RUN mv /go/src/2019-blind-2nd-elevator/elevator/logs /go/src/2019-blind-2nd-elevator/

EXPOSE 8000
CMD ./elevator
