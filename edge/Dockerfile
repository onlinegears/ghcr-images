FROM ghcr.io/onlinegears/gtk3:latest

RUN apt-get update \
	&& DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends \
		fonts-liberation \
		libatomic1 libdrm2 libgbm1 libnspr4 libnss3 \
		libu2f-udev mesa-vulkan-drivers \
		wget xdg-utils \
		libasound2 \
	&& apt-get clean \
	&& rm -rf /var/lib/apt/lists/*

RUN edge=microsoft-edge-stable_113.0.1774.57-1_amd64.deb \
	&& curl -O https://packages.microsoft.com/repos/edge/pool/main/m/microsoft-edge-stable/$edge \
	&& dpkg -i $edge \
	&& rm -f $edge
