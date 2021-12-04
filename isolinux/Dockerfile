FROM ghcr.io/onlinegears/base:latest

RUN apt-get update \
	&& DEBIAN_FRONTEND=noninteractive apt-get install -y \
		mkisofs xorriso cpio \
		isolinux \
	&& apt-get clean
