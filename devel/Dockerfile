FROM ghcr.io/onlinegears/base:latest

RUN apt-get update \
	&& DEBIAN_FRONTEND=noninteractive apt-get install -y \
		build-essential \
		autoconf \
		cmake \
		git \
		bison flex \
	&& apt-get clean
