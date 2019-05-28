FROM bellx2/rasbian-x86_64:stretch

LABEL maintainer="Bellx2 <bellx2@gmail.com>"

RUN apt-get update && \
	apt-get install -y nano
RUN apt-get install -y build-essential git \
    	libopencv-dev  libopencv-video-dev  libopencv-highgui-dev \
    	libssl-dev
RUN ln /dev/null /dev/raw1394
CMD ["/bin/bash"]
