FROM ubuntu:focal

ARG DEBIAN_FRONTEND=noninteractive
RUN apt-get update && \
    apt-get install -y gawk wget git-core diffstat unzip texinfo gcc-multilib \
    build-essential chrpath socat cpio python3 python3-pip python3-pexpect \
    xz-utils debianutils iputils-ping python3-git python3-jinja2 libegl1-mesa \
    libsdl1.2-dev pylint3 xterm python3-subunit mesa-common-dev \
    locales

RUN locale-gen en_US.UTF-8
ENV LANG en_US.UTF-8

RUN mkdir -p /workspace && chmod 777 /workspace

WORKDIR /workspace