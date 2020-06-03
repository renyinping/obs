FROM yinping/obs:base-ubuntu18.04

USER openwrt

WORKDIR /home/openwrt

RUN git clone https://www.github.com/openwrt/openwrt

WORKDIR /home/openwrt/openwrt

RUN ./scripts/feeds update -a &&\
    ./scripts/feeds install -a 

RUN wget https://github.com/renyinping/obs/raw/master/openwrt/.config &&\
    make download
