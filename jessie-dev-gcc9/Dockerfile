FROM bellx2/rasbian-x86_64:jessie-dev

LABEL maintainer="Ryu Tanabe <bellx2@gmail.com>"


RUN cd; git clone https://bitbucket.org/sol_prog/raspberry-pi-gcc-binary.git
RUN cd /opt; tar -xjvf ~/raspberry-pi-gcc-binary/gcc-9.1.0-armhf-raspbian.tar.bz2
RUN rm -rf ~/raspberry-pi-gcc-binary/
#RUN cp -R /opt/gcc-9.1.0/* /usr/
RUN cp -R /opt/gcc-9.1.0/lib/* /usr/lib/arm-linux-gnueabihf/
RUN ln /dev/null /dev/raw1394
CMD ["/bin/bash"]