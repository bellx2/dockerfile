FROM raspbian/jessie

LABEL maintainer="Ryu Tanabe <bellx2@gmail.com>"

# 非対話的インストールの設定
ARG DEBIAN_FRONTEND=noninteractive

RUN echo "deb http://archive.debian.org/debian/ jessie main" > /etc/apt/sources.list \
    && echo "deb http://archive.debian.org/debian-security jessie/updates main" >> /etc/apt/sources.list
RUN apt-get update && apt-get install -y --force-yes\
	nano \
	build-essential \
	git \
	libopencv-dev \
	libopencv-video-dev \
	libopencv-highgui-dev \
	libssl-dev \
	wget \
	curl \
&& apt-get clean \
&& rm -rf /var/lib/apt/lists/*

# WiringPiのインストール - curlを使用して直接ダウンロード
RUN curl -L -o /tmp/wiringpi.deb https://github.com/WiringPi/WiringPi/releases/download/2.61-1/wiringpi-2.61-1-armhf.deb \
    && dpkg -i /tmp/wiringpi.deb \
    && rm /tmp/wiringpi.deb

RUN ln /dev/null /dev/raw1394
CMD ["/bin/bash"]

