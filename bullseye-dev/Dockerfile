FROM bellx2/rasbian-x86_64:bullseye

LABEL maintainer="Ryu Tanabe <bellx2@gmail.com>"

RUN apt-get update && apt-get install -y \
	nano \
	build-essential git \
	libopencv-dev  libopencv-video-dev  libopencv-highgui-dev \
	libssl-dev \
	&& apt-get clean \
	&& rm -rf /var/lib/apt/lists/*
RUN wget https://project-downloads.drogon.net/wiringpi-latest.deb
RUN dpkg -i wiringpi-latest.deb
RUN rm wiringpi-latest.deb

RUN ln /dev/null /dev/raw1394
CMD ["/bin/bash"]
