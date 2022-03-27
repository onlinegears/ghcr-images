FROM ubuntu:latest

# Minimal tools and set Timezone
RUN apt-get update \
	&& DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends \
		ca-certificates \
		iproute2 \
		curl \
		file \
		vim \
		xz-utils \
		tzdata \
		less \
	&& apt-get clean \
	&& rm -rf /var/lib/apt/lists/* \
	&& ln -sf /usr/share/zoneinfo/Asia/Tokyo /etc/localtime
