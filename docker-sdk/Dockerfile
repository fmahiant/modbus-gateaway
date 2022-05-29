FROM alpine:latest
COPY  arm-buildroot-linux-uclibcgnueabihf_sdk-buildroot.tar.gz .
RUN tar xf arm-buildroot-linux-uclibcgnueabihf_sdk-buildroot.tar.gz -C /opt/ \
&& mv  /opt/arm-buildroot-linux-uclibcgnueabihf_sdk-buildroot/  /opt/cross-br-2022.02 && \
/opt/cross-br-2022.02/relocate-sdk.sh 