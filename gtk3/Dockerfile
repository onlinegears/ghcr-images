FROM ghcr.io/onlinegears/base:latest

RUN apt-get update \
	&& DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends \
		libgtk-3.0 \
                libx11-xcb1 x11-common \
	&& DEBIAN_FRONTEND=noninteractive apt-get install -y \
		locales-all fonts-noto \
	&& apt-get clean \
	&& rm -rf /var/lib/apt/lists/*
