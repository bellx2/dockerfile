FROM multiarch/ubuntu-core:arm64-xenial

LABEL maintainer="Ryu Tanabe <bellx2@gmail.com>"

ENV DEBIAN_FRONTEND=noninteractive

RUN apt-get update && apt-get install -y --no-install-recommends \
	nano \
	build-essential git \
  libopencv-dev libopencv-video-dev libopencv-highgui-dev \
	locales-all openssh-client ca-certificates \
	&& apt-get clean \
	&& rm -rf /var/lib/apt/lists/*
RUN git clone https://github.com/bats-core/bats-core.git
RUN cd bats-core; ./install.sh /usr/local; cd ..; rm -rf bats-core;
CMD ["/bin/bash"]
