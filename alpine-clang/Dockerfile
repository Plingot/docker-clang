ARG ALPINE_VERSION=3.15.0
FROM alpine:${ALPINE_VERSION}
LABEL maintainer="Mio Nilsson <mio@plingot.com>"
LABEL description="Alpine with cmake, clang and doxygen"

RUN apk add --no-cache \
  build-base \
  cmake \
  make \
  clang \
  clang-dev \
  llvm12 \
  pkgconf \
  pkgconfig \
  libc-dev \
  libstdc++ \
  binutils \
  file \
  doxygen \
  graphviz

RUN ln -sf /usr/bin/clang /usr/bin/cc
RUN ln -sf /usr/bin/clang++ /usr/bin/c++
