FROM ubuntu:18.04

WORKDIR /app

COPY . /app

RUN apt-get update \
	&& apt-get install -y gcc \
	&& apt-get install -y make \
	&& make

CMD ["./helloworld"]