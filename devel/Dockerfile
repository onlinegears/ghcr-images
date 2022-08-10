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
RUN curl -LO https://ziglang.org/download/0.9.1/zig-linux-x86_64-0.9.1.tar.xz \
	&& tar -Jxf zig-linux-x86_64-0.9.1.tar.xz -C /opt \
	&& rm zig-linux-x86_64-0.9.1.tar.xz
ENV PATH /usr/local/go/bin:/opt/zig-linux-x86_64-0.9.1:$PATH
