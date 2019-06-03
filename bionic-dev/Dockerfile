FROM multiarch/ubuntu-core:arm64-bionic

LABEL maintainer="Bellx2 <bellx2@gmail.com>"

ENV DEBIAN_FRONTEND=noninteractive

RUN apt-get update && \
	apt-get install -y nano
RUN apt-get install -y build-essential git \
    	libopencv-dev  libopencv-video-dev  libopencv-highgui-dev
CMD ["/bin/bash"]
