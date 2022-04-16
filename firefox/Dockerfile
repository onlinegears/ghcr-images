FROM ghcr.io/onlinegears/base:latest

RUN apt-get update \
	&& DEBIAN_FRONTEND=noninteractive apt-get install -y \
		dbus-x11 \
		locales locales-all \
		firefox firefox-locale-ja \
		fonts-noto \
	&& apt-get clean \
	&& rm -rf /var/lib/apt/lists/*
