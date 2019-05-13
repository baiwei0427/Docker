FROM ubuntu:18.04 AS builder

WORKDIR /build

COPY . /build

RUN apt-get update \
	&& apt-get install -y gcc \
	&& apt-get install -y make \
	&& make

FROM frolvlad/alpine-glibc

WORKDIR /app

RUN apk add glibc

COPY --from=builder /build/helloworld .

CMD ["./helloworld"]
