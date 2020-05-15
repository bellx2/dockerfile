FROM multiarch/ubuntu-core:arm64-bionic

LABEL maintainer="Ryu Tanabe<bellx2@gmail.com>"

ENV DEBIAN_FRONTEND=noninteractive
RUN apt-get update && apt-get install -y --no-install-recommends \
	nano \
	build-essential git \
  libopencv-dev libopencv-video-dev libopencv-highgui-dev \
	&& apt-get clean \
	&& rm -rf /var/lib/apt/lists/*

CMD ["/bin/bash"]
