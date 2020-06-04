FROM ubuntu:14.04

RUN apt-get update &&\
    apt-get install -y sudo build-essential ccache libncurses5-dev \
    zlib1g-dev gawk git subversion gettext libssl-dev xsltproc zip \
    vim nano curl wget python python3 file &&\
    apt-get clean &&\
    useradd -m openwrt &&\
    echo 'openwrt ALL=NOPASSWD: ALL' > /etc/sudoers.d/openwrt
