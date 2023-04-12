FROM ghcr.io/onlinegears/novnc:latest

RUN apt-get update \
	&& DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends \
		libgtk-3.0 \
		libx11-xcb1 x11-common \
	&& DEBIAN_FRONTEND=noninteractive apt-get install -y \
		bzip2 libasound2 libxtst6 libdbus-glib-1-2 \
	&& apt-get clean \
	&& rm -rf /var/lib/apt/lists/*

RUN curl -L -o /firefox-latest.tar.bz2 'https://download.mozilla.org/?product=firefox-latest-ssl&os=linux64&lang=ja' \
	&& tar -C /opt -jxf /firefox-latest.tar.bz2 \
	&& rm -rf /firefox-latest.tar.bz2
