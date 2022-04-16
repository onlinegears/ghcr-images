FROM ghcr.io/onlinegears/gtk3:latest

RUN apt-get update \
	&& DEBIAN_FRONTEND=noninteractive apt-get install -y \
		firefox firefox-locale-ja \
	&& apt-get clean \
	&& rm -rf /var/lib/apt/lists/*
