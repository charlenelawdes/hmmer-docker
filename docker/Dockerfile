FROM debian:bullseye

RUN apt-get update && apt-get install -y \
    git \
    gcc \
    python3 \
    python3-pip \
    wget \
    curl \
    unzip \
    htop \
    vim

RUN wget http://eddylab.org/software/hmmer/hmmer.tar.gz

RUN tar zxf hmmer.tar.gz

WORKDIR hmmer-3.4

RUN ./configure --prefix /usr/local

RUN make

RUN make install
