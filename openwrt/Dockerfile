FROM yinping/obs:base-ubuntu18.04

USER openwrt

WORKDIR /home/openwrt

RUN git clone https://www.github.com/openwrt/openwrt

WORKDIR /home/openwrt/openwrt

RUN ./scripts/feeds update -a &&\
    ./scripts/feeds install -a &&\
    make defconfig &&\
    make package/symlinks

RUN wget https://github.com/renyinping/obs/raw/master/openwrt/.config &&\
    make download &&\
    make tools/install &&\
    make toolchain/install &&\
    make target/compile
