FROM ghcr.io/onlinegears/devel:latest

RUN apt-get update \
	&& DEBIAN_FRONTEND=noninteractive apt-get install -y \
		cmake gcc-arm-none-eabi libnewlib-arm-none-eabi \
		python3-pip \
	&& apt-get clean
