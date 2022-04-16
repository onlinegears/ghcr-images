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
