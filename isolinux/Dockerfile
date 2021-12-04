FROM ghcr.io/onlinegears/base:latest

RUN apt-get update \
	&& DEBIAN_FRONTEND=noninteractive apt-get install -y \
		mksiofs xorriso cpio \
		isolinux \
	&& apt-get clean
