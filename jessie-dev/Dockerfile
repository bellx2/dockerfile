FROM bellx2/rasbian-x86_64:jessie

LABEL maintainer="Ryu Tanabe <bellx2@gmail.com>"

RUN apt-get update && apt-get install -y \
	nano \
	build-essential \
	git \
	libopencv-dev \
	libopencv-video-dev \
	libopencv-highgui-dev \
	libssl-dev \
	wiringpi \
&& apt-get clean \
&& rm -rf /var/lib/apt/lists/*

RUN ln /dev/null /dev/raw1394
CMD ["/bin/bash"]

