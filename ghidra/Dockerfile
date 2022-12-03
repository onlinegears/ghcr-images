FROM ghcr.io/onlinegears/devel:latest

RUN apt-get update \
	&& DEBIAN_FRONTEND=noninteractive apt-get install -y \
		openjdk-11-jdk \
		zip \
	&& apt-get clean

RUN (cd /opt; \
	curl -LO https://github.com/NationalSecurityAgency/ghidra/releases/download/Ghidra_10.2.2_build/ghidra_10.2.2_PUBLIC_20221115.zip; \
	unzip ghidra_10.2.2_PUBLIC_20221115.zip; \
	rm -f ghidra_10.2.2_PUBLIC_20221115.zip; \
	ln -sf ghidra_10.2.2_PUBLIC ghidra)
