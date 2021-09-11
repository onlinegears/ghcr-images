FROM ubuntu:latest

# Minimal tools
RUN apt-get update \
	&& DEBIAN_FRONTEND=noninteractive apt-get install -y \
		ca-certificates \
		iproute2 \
		curl \
		file \
		vim \
		xz-utils \
		tzdata \
		less \
	&& apt-get clean
# Timezone
RUN ln -sf /usr/share/zoneinfo/Asia/Tokyo /etc/localtime
