FROM ubuntu:latest

LABEL \
  version="0.1.2" \
  description="Speedseq: A flexible framework for rapid genome analysis and interpretation"

RUN apt-get update && apt-get install -y tar gzip bzip2 \
  python-pip \
  python-dev \
  build-essential \
  cmake \
  git \
  libtool \
  zlib1g-dev \
  gawk \
  libbz2-dev \
  liblzma-dev \
  libncurses5-dev \

RUN apt-get install -y  python-numpy python-scipy 

RUN pip install --upgrade pip && pip install pysam 
  
RUN  git clone --recursive https://github.com/hall-lab/speedseq \
&& cd /speedseq/ \
&& make


CMD ["/bin/bash"]
