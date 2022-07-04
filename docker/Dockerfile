# Build:
#   docker build --rm -t tandem -f ./docker/Dockerfile .
FROM nvidia/cuda:11.3.1-devel-ubuntu20.04

ARG DEBIAN_FRONTEND=noninteractive

RUN apt update && apt upgrade
RUN apt update && apt install -y \
    wget git libsuitesparse-dev libeigen3-dev libboost-all-dev \
    libopencv-dev

RUN wget https://download.pytorch.org/libtorch/cu111/libtorch-cxx11-abi-shared-with-deps-1.9.0%2Bcu111.zip
