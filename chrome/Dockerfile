FROM ghcr.io/onlinegears/gtk3:latest

RUN apt-get update \
	&& DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends \
		fonts-liberation \
		libdrm2 libgbm1 libnspr4 libnss3 \
		wget xdg-utils \
	&& apt-get clean \
	&& rm -rf /var/lib/apt/lists/*

RUN curl -O https://dl.google.com/linux/direct/google-chrome-stable_current_amd64.deb \
	&& dpkg -i google-chrome-stable_current_amd64.deb \
	&& rm -f google-chrome-stable_current_amd64.deb
