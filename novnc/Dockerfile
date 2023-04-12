FROM ghcr.io/onlinegears/base:latest

RUN apt-get update \
	&& DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends \
		lxde xdg-utils \
	&& DEBIAN_FRONTEND=noninteractive apt-get install -y \
		locales-all fonts-noto \
		fcitx-mozc \
		tigervnc-standalone-server \
		novnc websockify \
	&& apt-get clean \
	&& rm -rf /var/lib/apt/lists/*
