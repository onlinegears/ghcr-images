FROM ghcr.io/onlinegears/base:latest

RUN apt-get update \
	&& DEBIAN_FRONTEND=noninteractive apt-get install -y \
		build-essential \
		autoconf \
		cmake \
		git \
		bison flex nasm \
		strace gdb \
	&& apt-get clean \
	&& rm -rf /var/lib/apt/lists/*
RUN curl -vLO https://go.dev/dl/go1.18.3.linux-amd64.tar.gz \
	&& tar -zxf go1.18.3.linux-amd64.tar.gz -C /usr/local \
	&& rm go1.18.3.linux-amd64.tar.gz
ENV PATH /usr/local/go/bin:$PATH
