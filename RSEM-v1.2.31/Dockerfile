FROM ubuntu:latest

RUN apt-get update && apt-get install -y tar gzip bzip2 \
  git \
  build-essential \
  python-dev 
  
RUN  git clone https://github.com/deweylab/RSEM.git \
  && cd /RSEM/ \
  && make \
  && make install


CMD ["/bin/bash"]
