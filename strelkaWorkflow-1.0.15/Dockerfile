FROM ubuntu:latest

LABEL \
  version="1.0.15" \
  description="StrelkaWorkflow for somatic mutation detection"

RUN apt-get update && apt-get install -y  tar gzip \
  bzip2 \
  g++ \
  make \
  perl-doc \
  python \
  rsync \
  wget \
  zlib1g-dev
  
RUN  wget --no-check-certificate https://sites.google.com/site/strelkasomaticvariantcaller/home/download/strelka_workflow-1.0.15.tar.gz \
  && tar -zxvf strelka_workflow-1.0.15.tar.gz \
  && rm -f strelka_workflow-1.0.15.tar.gz \
  && cd /strelka_workflow-1.0.15 \
  && ./configure \
  && make \
  && make install \
  && cp /strelka_workflow-1.0.15/etc/strelka_config_isaac_default.ini /opt/config.ini 

CMD ["/bin/bash"]
