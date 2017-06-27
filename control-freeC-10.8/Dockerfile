FROM ubuntu:latest

RUN apt-get update && apt-get install -y \
  wget \
  make \
  g++ \
  r-base \
  r-base-dev
  
RUN  wget https://github.com/BoevaLab/FREEC/archive/v10.8.tar.gz \
  && tar -zxvf v10.8.tar.gz \
  && rm -r v10.8.tar.gz \
  && chmod 755 /FREEC-10.8/



CMD ["/bin/bash"]
