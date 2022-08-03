FROM ghcr.io/onlinegears/devel:latest

RUN apt-get update \
	&& DEBIAN_FRONTEND=noninteractive apt-get install -y \
		openjdk-11-jdk \
		zip \
	&& apt-get clean

RUN (cd /opt; \
	curl -LO https://github.com/NationalSecurityAgency/ghidra/releases/download/Ghidra_10.1.5_build/ghidra_10.1.5_PUBLIC_20220726.zip; \
	unzip ghidra_10.1.5_PUBLIC_20220726.zip; \
	rm -f ghidra_10.1.5_PUBLIC_20220726.zip; \
	ln -sf ghidra_10.1.5_PUBLIC ghidra)
