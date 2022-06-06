FROM ubuntu:22.04
RUN apt-get update
RUN apt-get -qq -y install gettext sed grep file bash cmake build-essential pkg-config
COPY  arm-buildroot-linux-uclibcgnueabihf_sdk-buildroot.tar.gz .
RUN tar xf arm-buildroot-linux-uclibcgnueabihf_sdk-buildroot.tar.gz -C /opt/ \
&& mv  /opt/arm-buildroot-linux-uclibcgnueabihf_sdk-buildroot/  /opt/cross-br-2022.02 && \
/opt/cross-br-2022.02/relocate-sdk.sh
WORKDIR /code
ENTRYPOINT [ "bash" ]