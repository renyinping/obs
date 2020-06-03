FROM yinping/obs:base-ubuntu18.04

RUN sudo -iu openwrt bash &&\
    git clone https://www.github.com/openwrt/openwrt

RUN cd openwrt &&\
    ./scripts/feeds update -a &&\
    ./scripts/feeds install -a

