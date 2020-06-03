FROM yinping/obs:openwrt

RUN sudo -iu openwrt bash &&\
    cd openwrt &&\
    git pull &&\
    ./scripts/feeds update -a
